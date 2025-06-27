<!-- Plugin description -->
![Context Mapper](https://raw.githubusercontent.com/wiki/ContextMapper/context-mapper-dsl/logo/cm-logo-github-small.png)
# Context Mapper IntelliJ Plugin

> **_NOTE:_** This plugin is a proof of concept. It does not support all Context Mapper features yet.

[![IntelliJ Plugin Build](https://github.com/ContextMapper/context-mapper-intellij-plugin/actions/workflows/build.yml/badge.svg)](https://github.com/ContextMapper/context-mapper-intellij-plugin/actions/workflows/build.yml) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=ContextMapper_context-mapper-intellij-plugin&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=ContextMapper_context-mapper-intellij-plugin) [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

[Context Mapper](https://contextmapper.org/) is an open source tool providing a Domain-specific Language based on Domain-Driven Design (DDD) patterns for context mapping and service decomposition.

## System Requirements
To use the Context Mapper IntelliJ plugin you need the following tools (besides IntelliJ and our extension) installed locally:

* [Oracle Java](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) or [OpenJDK](https://openjdk.java.net/) (JRE 11 or newer)
* [Node.js](https://nodejs.org/en/download) (v22)
* Maybe you want to install a [PlantUML extension](https://plugins.jetbrains.com/plugin/7017-plantuml-integration) for the generated PlantUML diagrams.
* LSP4IJ IntelliJ plugin (will be installed automatically when installing our plugin)

<!-- Plugin description end -->

## Build and/or Run Extension Locally
This project uses [Gradle](https://gradle.org/) to build the IntelliJ plugin.

### Requirements
To be able to work on the plugin in IntelliJ, you need to have the [Plugin DevKit](https://plugins.jetbrains.com/plugin/22851-plugin-devkit) plugin installed.

The language server package is downloaded from the GitHub NPM registry, which requires you to provide an authentication token.
You can get a token by creating a [personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens) in your GitHub account.
Make sure that the token includes the **package:read** permission.

To configure the registry and authentication, add this configuration to the `.npmrc` file in your home directory.
```
@contextmapper:registry=https://npm.pkg.github.com
//npm.pkg.github.com/:_authToken=<TOKEN>
```

### Commands
After cloning this repository, you can build the project with the following command:

```bash
./gradlew clean buildPlugin
```

Use the following command to build and run the plugin:

```bash
./gradlew runIde
```

## Contributing
Contribution is always welcome! Here are some ways how you can contribute:
* Create Github issues if you find bugs or just want to give suggestions for improvements.
* This is an open source project: if you want to code, [create pull requests](https://help.github.com/articles/creating-a-pull-request/) from [forks of this repository](https://help.github.com/articles/fork-a-repo/). Please refer to a Github issue if you contribute this way.
* If you want to contribute to our documentation and user guides on our website [https://contextmapper.org/](https://contextmapper.org/), create pull requests from forks of the corresponding page repo [https://github.com/ContextMapper/contextmapper.github.io](https://github.com/ContextMapper/contextmapper.github.io) or create issues [there](https://github.com/ContextMapper/contextmapper.github.io/issues).

## Licence
ContextMapper is released under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).
