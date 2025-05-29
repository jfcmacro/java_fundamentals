# Session 03. Maven Build Tools

## Java Project Management 

* Ant
* Maven
* Gradle

---

## Java Project Management - Maven

### Introducing Apache Maven

* Convention over configuration.
* Maven incorporates the concept by providing sensible default behaviors for projects.
* Maven is based on plugins that describe the life cycle.
* Conceptual Model of a Project
  * Dependency Management
  * Remote Repositories
  * Universal reuse of build logic
  * Tool portability and integration
  * Easy searching and filtering of project artifacts

---

## Java Project Management - Maven

### Creating A Simple Maven Project

Type the next command to create a new maven project:

```shell
$ mvn archetype:generate -DgroupId=org.sonatype.mavenbook \
    -DartifacId=simple -Dpackage=org.sonatype.mavenbook \
    -Dversion=1.0-SNAPSHOT
```

That command will ask you which archetype must be launched (By default `maven-archetype-quickstart`)

A longer command is the next one:

```shell
$ mvn archetype:generate -DgroupId=org.sonatype.mavenbook -DartifactId=simple \
     -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 \ 
     -Dpackage=org.sonatype.mavenbook -DinteractiveMode=false
```

The following folder hierarchies are created:

![image-20240223184708823](.\images\image-20240223184708823.png)

-------------------------------------------------------------------------------

## Java Project Management - Maven Lifecycle

- `validate` - validate the project is correct and all necessary information is available
- `compile` - compile the source code of the project
- `test` - test the compiled source code using a suitable unit testing framework. These tests should not require the code to be packaged or deployed
- `package` - package the compiled code in its distributable format, such as a JAR.
- `verify` - run any checks on results of integration tests to ensure quality criteria are met
- `install` - install the package into the local repository, for use as a dependency in other projects locally
- `deploy` -  this is done in the build environment, copies the final package to the remote repository for sharing with other developers and projects.

