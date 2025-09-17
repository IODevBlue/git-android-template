(Title)
=========================

[![Current Version](https://img.shields.io/github/v/tag/IODevBlue/:repo?label=Current%20Version&color=2CCCE4&style=for-the-badge&labelColor=0109B6)](https://github.com/IODevBlue/:repo/releases)
[![Repo Size](https://img.shields.io/github/repo-size/IODevBlue/:repo?color=2CCCE4&style=for-the-badge&labelColor=0109B6)](https://github.com/IODevBlue/:repo)
[![License](https://img.shields.io/github/license/IODevBlue/:repo?color=2CCCE4&style=for-the-badge&labelColor=0109B6)](http://www.apache.org/licenses/LICENSE-2.0)
[![Stars](https://img.shields.io/github/stars/IODevBlue/:repo?color=2CCCE4&style=for-the-badge&labelColor=0109B6)](https://github.com/IODevBlue/:repo/stargazers)
[![Gradle](https://img.shields.io/static/v1?label=Gradle&message=9.0.0&color=2CCCE4&style=for-the-badge&labelColor=0109B6)](https://docs.gradle.org/9.0.0/release-notes)
[![Kotlin](https://img.shields.io/static/v1?label=Kotlin&message=2.2.20&color=2CCCE4&style=for-the-badge&labelColor=0109B6)](https://kotlinlang.org/docs/whatsnew2220.html)

Table of content
----------------
- [Documentations](https://github.com/IODevBlue/:repo/tree/main#documentations)
- [Uses](https://github.com/IODevBlue/:repo/tree/main#uses)
- [Features](https://github.com/IODevBlue/:repo/tree/main#features)
- [Installation](https://github.com/IODevBlue/:repo/tree/main#installation)
- [Usage](https://github.com/IODevBlue/:repo/tree/main#usage)
- [Java interoperability](https://github.com/IODevBlue/:repo/tree/main#java-interoperability)
- [Configurations](https://github.com/IODevBlue/:repo/tree/main#configurations)
  - [XML attributes](https://github.com/IODevBlue/:repo/tree/main#xml-attributes)
- [Applications using :repo](https://github.com/IODevBlue/:repo/tree/main#applications-using-:repo)
- [Contributions](https://github.com/IODevBlue/:repo/tree/main#contributions)
- [Changelog](https://github.com/IODevBlue/:repo/tree/main#changelog)
- [License](https://github.com/IODevBlue/:repo/tree/main#license)


Dependencies (Optional)
-----------------------

Documentations
--------------
Documentations are available online in [Javadoc](https://raw.githack.com/IODevBlue/project-docs/main/api/android/:repo/javadoc/index.html) and [KDoc](https://raw.githack.com/IODevBlue/project-docs/main/api/android/:repo/html/index.html).

Uses
----

(Then add illustrative photographs after the break above)
<p style="text-align: center;">
  <img src="/art/placeholder.png" alt="name"
></p>


Features (Optional)
--------



Installation
------------
**current-version: ---**

There are several ways to install this library.

Grab a JAR artifact from the Maven Central Repository:
- Using Kotlin DSL.
```kotlin
//build.gradle.kts
implementation ("io.github.iodevblue::repo:${current-version}")
```
- Using Groovy DSL.
```groovy
//build.gradle
implementation 'io.github.iodevblue::repo:$current-version'
```
- On Apache Maven
```XML
<dependency>
  <groudId> io.github.iodevblue </groudId>
  <artifactId> id </artifactId>
  <version> :repo </version>
</dependency>
```
- If it is a snapshot version, add the snapshot Maven Nexus OSS repository:
  - Using Kotlin DSL
  ```kotlin
  //build.gradle.kts
  maven {
    url = uri("https://central.sonatype.com/repository/maven-snapshots/")
  }
  ```
  - Using Groovy DSL
  ```groovy
  //build.gradle
   maven {
        url "https://central.sonatype.com/repository/maven-snapshots/"
    }
  ```
- Then retrieve a copy:
```kotlin
//build.gradle.kts
implementation ("io.github.iodevblue::repo:${current-version}-SNAPSHOT")
```

Grab a `JAR` or `AAR` artifact from the [release](https://github.com/IODevBlue/:repo/releases) section.

Place it in `libs` directory in your project module and install in your project.
  - Using Kotlin DSL
  ```kotlin
  //build.gradle.kts
  implementation(fileTree("libs") { include("*.jar", "*.aar") })
  ```
  - Using Groovy DSL
  ```groovy
  //build.gradle
  implementation(fileTree("libs") { include("*.jar", "*.aar") })
  ```
- The `libs` directory should be inside your module directory **not** the root project directory.
  For example, if your module is `app`:
  ```text
  YourProject/
  ├── app/
  │   ├── src/
  │   ├── build.gradle.kts (or build.gradle)
  │   └── libs/
  │       ├── :repo_v$current-version.jar
  │       └── :repo_v$current-version.aar
  └── settings.gradle.kts
  ```

Usage
-----

Java Interoperability (Optional: For Kotlin projects)
---------------------

Configurations (Optional)
---------------
| Variable   |    Default    | Use                        |
|:-----------|:-------------:|:---------------------------|
| `varName`  | Default Value | Use (as in documentation). |

Methods (Optional)
---------------
| Method     |    Returns    | Use                        |
|:-----------|:-------------:|:---------------------------|
| `method()` |  Return Type  | Use (as in documentation). |

XML Attributes (Optional)
---------------
| Attribute  |    Default    | Use                        |
|:-----------|:-------------:|:---------------------------|
| `varName`  | Default Value | Use (as in documentation). |


Applications using :repo (Optional)
------------------------
If your application uses :repo and you'd love to showcase, send an <a href="mailto:iodevblue@gmail.com">email</a> containing:
- An app icon
- A link to download your application.
- A related Github repository.

Contributions
-------------
Contributors are welcome!

**NOTE:** This repository is organized into two branches:
- [main](https://github.com/IODevBlue/:repo/tree/main) branch: contains stable, finalized updates.
- [development](https://github.com/IODevBlue/:repo/tree/development) branch: used for active development and proposed changes.

Check the [Contributing](https://github.com/IODevBlue/:repo/blob/development/CONTRIBUTING.md) for more information.


Changelog
---------
* **1.0.0**
    * Initial release

Check the [CHANGELOG](https://github.com/IODevBlue/:repo/blob/main/CHANGELOG.md) for all previous releases..


License
=======
```
    Copyright 2025 IO DevBlue

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
```