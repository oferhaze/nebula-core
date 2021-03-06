Nebula Plugins
=============
The nebula-plugins organization was setup to facilitate the generation, governance, and releasing of Gradle plugins.

Guidelines:
* Should be named gradle-*-plugin. Can use nebula-*-plugin for opinionated plugins.
* Plugin’s name will be the asterisk above, except for nebula-*-plugin’s which are named nebula-*
* Should have a branch and releases for major Gradle versions
* Version prefix needs to be the short version of Gradle, e.g. 1.8.0 for Gradle 1.8 support
* All plugins will apply a core plugin to centralize publishing
* Plugins will publish to bintray.com
* Plugins will have Cloudbee Jenkins jobs for building and releasing, to allow anyone to publish a release.
* Plugins will use the Apache 2.0 license, enforced via license plugin
* Development should be done via pull requests, which can be done on feature branches
* Pull requests should be review by someone who isn't the author

Nebula Core
===========
This specific project holds some "helper" classes for testing and interacting with Gradle. It's not meant to get too big, 
but should serve as a central place for all plugins. This project should have no dependency and not contain any specific
plugins.

TODO
----------
Create a test configuration for test code.


