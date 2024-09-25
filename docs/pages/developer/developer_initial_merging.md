
> **Summary:** Getting started as a developer.

This document will walk you through your first contribution to the Interlok codebases.

## Prerequisites.

1) Install GIT, latest version
2) Have or create a github account
3) Ask for "contributor" access or to be added to the _uk_dev_ github group.

## Pre-check in

The Interlok development team use gitflow with all check-ins, so before you make any code changes, make sure you are on the _develop_ branch of the project you're working on.
Next you must make sure your code base is up-to-date, so pull/sync any changes from github to your local copy.

Assuming you have now made your code changes, you'll need to post a commit.
Do make sure you do not commit to the _develop_ branch, normally this branch is protected and will not allow you to push to.  Simply create a new branch, usually with the Jira ticket ID as the name of the branch, then commit your changes to this new branch.

Before pushing your changes, you can re-sync your new branch with that on the develop branch in github, just in-case there are further changes which should make your code merge easier.

Push your changes branch to github.

## Creating a merge request

Once you've pushed your branch you can login to github.com, find your project and create a merge request through the web UI.
The moment you create your merge request a templated check-list will be generated.  The check-list is a fairly comprehensive list you'll need to confirm.  Perhaps not all items on the list will be applicable to your check-in, but do run through the list to make sure nothing has been forgotten.

The new merge request will automatically perform a build, run the full unit test suite, perform a code check, make sure the code coverage has not dropped and check for dependency vulnerabilities.  Assuming these checks pass, you'll need to assign an authorized user to review your changes.

From this moment you'll keep an eye on your merge request for any comments and any requests for change.  Assuming your merge request is approved you can now merge your branch into the develop branch.