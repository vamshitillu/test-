# Basic Maven Project

This is a basic Maven-based Java project created with the [Library Maven Archetype](https://github.com/Bernardo-MG/library-maven-archetype).

It comes ready to follow several good practices, such as the use of continuous integration, unit/integration testing or the creation of documentation with the use of Maven Site.

While the archetype is meant to help start building the project quickly, there are a few things which may be a good idea to check and, if needed, change:

- This readme's description
- Project info on the POM
- The documentation on the project's Maven site
- License, if not using the MIT one (POM, readme and LICENSE files)
- Links on the readme, POM and Maven site (repositories, issues, etc)

Note that the Maven site documentation (found at /src/site) will require the most work, as there is where the library's documentation, or at least a basic version of it, meant to go. Check the [Maven Site](https://maven.apache.org/plugins/maven-site-plugin/) home, and the [Docs Maven Skin](https://github.com/Bernardo-MG/docs-maven-skin), which is the Maven skin being used, for information about how to edit it.

[![Maven Central](https://img.shields.io/maven-central/v/sravani1/rvr.svg)][maven-repo]
[![Bintray](https://api.bintray.com/packages/bernardo-mg/maven/rvr/images/download.svg)][bintray-repo]

[![Release docs](https://img.shields.io/badge/docs-release-blue.svg)][site-release]
[![Development docs](https://img.shields.io/badge/docs-develop-blue.svg)][site-develop]

[![Release javadocs](https://img.shields.io/badge/javadocs-release-blue.svg)][javadoc-release]
[![Development javadocs](https://img.shields.io/badge/javadocs-develop-blue.svg)][javadoc-develop]

## Features

The project by default comes with a useful series of features:

- Preconfigured to begin developing a new library fast.
- Prepared for continuous integration, which differentiates between development and release artifacts and documentation.
- Unit and integration tests suites ready to be run with [TestNG](http://testng.org/).
- A Maven site, using the [Docs Maven Skin](https://github.com/Bernardo-MG/docs-maven-skin), ready to show documentation and several reports.
- Various useful files, such as readme, gitignore and gitattributes.

## Documentation

Documentation is always generated for the latest release, kept in the 'master' branch:

- The [latest release documentation page][site-release].
- The [the latest release Javadoc site][javadoc-release].

Documentation is also generated from the latest snapshot, taken from the 'develop' branch:

- The [the latest snapshot documentation page][site-develop].
- The [the latest snapshot Javadoc site][javadoc-develop].

The documentation site sources come along the source code (as it is a Maven site), so it is always possible to generate them using the following Maven command:

```
$ mvn verify site
```

The verify phase is required, as otherwise some of the reports won't be created.

## Usage

The application is coded in Java, using Maven to manage the project.

### Prerequisites

The project has been tested on the following Java versions:
* JDK 7
* JDK 8
* OpenJDK 7

All other dependencies are handled through Maven, and noted in the included POM file.

### Installing

The recommended way to install the project is by setting up your preferred dependencies manager. To get the configuration information for this check the [Bintray repository][bintray-repo], or the [Maven Central Repository][maven-repo].

If for some reason manual installation is necessary, just use the following Maven command:

```
$ mvn install
```

## Collaborate

Any kind of help with the project will be well received, and there are two main ways to give such help:

- Reporting errors and asking for extensions through the issues management
- or forking the repository and extending the project

### Issues management

Issues are managed at the GitHub [project issues tracker][issues], where any Github user may report bugs or ask for new features.

### Getting the code

If you wish to fork or modify the code, visit the [GitHub project page][scm], where the latest versions are always kept. Check the 'master' branch for the latest release, and the 'develop' for the current, and stable, development version.

## License

The project has been released under the [MIT License][license].

[bintray-repo]: https://bintray.com/bernardo-mg/maven/rvr/view
[maven-repo]: http://mvnrepository.com/artifact/sravani1/rvr
[issues]: https://github.com/bernardo-mg/rvr/issues
[javadoc-develop]: http://docs.wandrell.com/development/maven/rvr/apidocs
[javadoc-release]: http://docs.wandrell.com/maven/rvr/apidocs
[license]: http://www.opensource.org/licenses/mit-license.php
[scm]: https://github.com/bernardo-mg/rvr
[site-develop]: http://docs.wandrell.com/development/maven/rvr
[site-release]: http://docs.wandrell.com/maven/rvr
