
# Introduction

> **Summary:** The config page allows you to configure your Interlok container in an easy to use graphically way. Basically, it's a UI way of editing the adapter.xml that controls how the Interlok container behaves. Using this page, you can apply changes to your running container; you can add, edit and delete components such as consumers, producers, services, etc. The UI application will also validate your changes, show you inline help during your editing and allows you to insert components from pre-defined templates.

### Important to Understand ###

Before working with the config page, it’s important to understand that there is a divorce between the config page (and projects) and the running adapters config.

When you are using the config page, you are not editing live adapter config on the running adapter. You are editing a stored configuration xml file, which is either stored in the [default ui store](/pages/ui/ui-saved-config-projects) or saved on your [local file system](/pages/ui/ui-saved-config-projects#save-a-config-project) or saved on a remote [version control system](/pages/ui/ui-version-control).

The config changes are *not* ‘made live’ until you [apply](/pages/ui/ui-config#applying-a-configuration) them to a given running adapter.

When you navigate to the config page, it’s important to understand that it will always attempt to [load the active](/pages/ui/ui-user-preferences#configuration-page-preferences) adapters config (if only one adapter is registered with the ui) if you have this user preference set to true. If this is set to false, then the page will attempt to reopen the [project](/pages/ui/ui-config-project) you were working on (within the browser session). This is very important to understand, otherwise you may be editing config loaded from the running adapter rather than the project you are working on.

It’s recommended that if you indeed to use ui projects, that you turn the auto load user preference to false.
