# Fully integrating Optional Components in the UI

> **Summary:** Interlok 3.5.0 introduced the [Optional Component Discovery Page](/pages/ui/ui-optional-component-discovery) which is build dynamically from data obtained from the [Adaptris Nexus Instance](https://nexus.adaptris.net/nexus) and the optional projects individual pom.xml files. This page is for component developers who want to fully integrate their optional components with the UI.

?> The details on this page are correct for Interlok version 3.11.1-RELEASE/3.12-SNAPSHOT

## The Optional Components List ##

?> The UI [Optional Component Discovery Page](/pages/ui/ui-optional-component-discovery) will not work if you have [Disabled External Resources](/pages/ui/ui-system-preferences)

During the UI startup, where Interloks built-in jetty starts the ui and executes our initialisation servlets, the optional components list and details are loaded and cached. 

This is all done by querying a nexus API. It is executed during startup as it can sometimes be slow, as it is an external callout, and we cache the results so the optional page usable immediately.

The default nexus instance that the UI uses is: https://nexus.adaptris.net/nexus

The initial list of optional components is loaded by using the following query:

```
${nexus-base}/service/local/lucene/search?repositoryId=${repository}&g=com.adaptris&v=${artifact-version}&p=jar
```

The variables explained:
* ${nexus-base} This is the URL to the Nexus instance that we want to query, i.e. https://nexus.adaptris.net/nexus
* ${repository} In Nexus there are many repositories, for example 'releases' or 'snapshots', so we need to specify which one we aerr querying
* ${artifact-version} Which versions are we attempting to list, i.e. 3.12-SNAPSHOT, 3.11.1-RELEASE, 3.10.0B1-RELEASE etc.

The UI version will dictate the initial values for the initial list to be loaded.

For example, if you started a Interlok 3.11.1 release, the UI would query:
```
https://nexus.adaptris.net/nexus/service/local/lucene/search?repositoryId=releases&g=com.adaptris&v=3.11.1-RELEASE&p=jar
```

But if you started a Interlok 3.12 snapshot, the UI would query:
```
https://nexus.adaptris.net/nexus/service/local/lucene/search?repositoryId=snapshots&g=com.adaptris&v=3.12-SNAPSHOT&p=jar
```

This query returns XML, such as:
```xml
<searchNGResponse>
    <repoDetails>
        <NexusNGRepositoryDetail>
            <repositoryId>releases</repositoryId>
            <repositoryName>Adaptris Public Releases</repositoryName>
        </NexusNGRepositoryDetail>
    </repoDetails>
    <data>
        <artifact>
            <groupId>com.adaptris</groupId>
            <artifactId>interlok-fx-installer</artifactId>
            <version>3.11.1-RELEASE</version>
            <latestRelease>3.11.1-RELEASE</latestRelease>
            <latestReleaseRepositoryId>releases</latestReleaseRepositoryId>
        </artifact>  
        <!-- a whole load of these artifact elements, one per optional component, current count is 115 -->
    </data>
</searchNGResponse>
```

And parsing this XML response, the UI knows what optional components it needs to load and display.
The Xpath used:
```
/searchNGResponse/data/artifact/artifactId/text()
```

?> **NOTE** On the 'Optional Component Discovery Page' you can edit the list query variables and reload the components by clicking the page settings, via the 'cog' icon and editting the default settings. This way you can browse component lists from previous/future release/snapshot versions without changing your current UI version. 

The 'Optional Component Discovery Page' settings button:

![optional components settings button](../../images/developer/developer-ui-optional-components-settings-button.png)

The 'Optional Component Discovery Page' settings modal:

![optional components settings modal](../../images/developer/developer-ui-optional-components-settings-modal.png)

## Log4j ##

If you need to see the log statements for the UI optional component loading, you can add this to your log4j configuration:
```xml
    <Logger name="com.adaptris.adaptergui.initialisation.impl.InitOptionalComponentServiceImpl" level="TRACE"/>
    <Logger name="com.adaptris.adaptergui.service.impl.OptionalComponentServiceImpl" level="TRACE"/>
    <Logger name="com.adaptris.adaptergui.util.OptionalComponentCache" level="TRACE"/>
```

## The Optional Components Details ##




