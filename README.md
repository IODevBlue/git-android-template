(Title)
=========================

[<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/IODevBlue/:repo?label=Current Version&color=2CCCE4&style=for-the-badge&labelColor=0109B6">](https://github.com/IODevBlue/:repo/releases) <img alt="Repository Size" src="https://img.shields.io/github/repo-size/IODevBlue/:repo?color=2CCCE4&style=for-the-badge&labelColor=0109B6"> [<img alt="License" src="https://img.shields.io/github/license/IODevBlue/:repo?color=2CCCE4&style=for-the-badge&labelColor=0109B6">](http://www.apache.org/licenses/LICENSE-2.0) [<img alt="GitHub Repository stars" src="https://img.shields.io/github/stars/IODevBlue/:repo?color=2CCCE4&style=for-the-badge&labelColor=0109B6">](https://github.com/IODevBlue/:repo/stargazers)
<img alt="GitHub watchers" src="https://img.shields.io/github/watchers/IODevBlue/:repo?label=Repository Watchers&color=2CCCE4&style=for-the-badge&labelColor=0109B6"> [<img alt="Gradle version" src="https://img.shields.io/static/v1?label=Gradle version&message=8.0.0&color=2CCCE4&style=for-the-badge&labelColor=0109B6">](https://docs.gradle.org/8.0/release-notes) [<img alt="Kotlin version" src="https://img.shields.io/static/v1?label=Kotlin version&message=1.8.20&color=2CCCE4&style=for-the-badge&labelColor=0109B6">](https://KOTLINlang.org/docs/whatsnew1820.html)

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
<p align="center"><img src="/art/square1.png" alt="name"></p>


Features (Optional)
--------



Installation
------------
**current-version: ---**

There are several ways to install this library.

1. Grab a JAR artifact from the Maven Central Repository:
```GROOVY
implementation 'io.github.iodevblue::repo:1.0.0'
```
- On Apache Maven
```XML
<dependency>
  <groudId> io.github.iodevblue </groudId>
  <artifactId> id </artifactId>
  <version> :repo </version>
</dependency>
```
If it is a snapshot version, add the snapshot Maven Nexus OSS repository:
```GROOVY
maven {   
  url 'https://s01.oss.sonatype.org/content/repositories/snapshots/'
}
```
Then retrieve a copy:
```GROOVY
implementation 'io.github.iodevblue::repo:1.0.0-SNAPSHOT'
```

2. Grab a JAR or AAR artifact from the [release](https://github.com/IODevBlue/:repo/releases) section.
- Place it in `libs` folder in your project module and install in your project.
```GROOVY
implementation fileTree(dir:' libs', include:'*jar')
```

If you do not prefer the compiled JAR and want access to the source files directly:

3. [Download](https://github.com/IODevBlue/:repo/archive/refs/heads/main.zip) the project zip file.
- Create a new module with name `:repo` in your project.
- Copy the contents of the `library` module from the downloaded project zip file to the new module `:repo`.
- This method makes the source code accessible. If you do make major or minor improvements to the source code, consider making a pull request or an issue to make a contribution.
Check the [Contributing](https://github.com/IODevBlue/:repo/blob/development/CONTRIBUTING.md) for more information.

4. If creating a new module is not preferable for your project and you want to have access to the source codes while tightly coupling it to your project, then follow this process:
- [Download](https://github.com/IODevBlue/:repo/archive/refs/heads/main.zip) the project zip file.
- Create a new package with name `:repo` in your project.
- Copy the subpackages and class files from the `com.blueiobase.api.android.:repo` package from the downloaded project zip file into the new `:repo` package.
- Edit the package declaration in each class file accordingly.
- Copy the contents of the `res` folder in the project zip into your module's `res` folder. 
- Alternatively for convenience and arrangement in an ordered manner, you could create a `sourceSet` dedicated to 3rd party libraries like so:
```GROOVY
android {
  sourceSets {
    main {
      res {
        srcDirs file("src/main/thirdpartyres/").listFiles(),
                'src/main/thirdpartyres'
      }
      java {
        srcDirs 'src/main/thirdpartylibraries'
      }
    }
  }
}
```
- Then sync project with Gradle.
- This creates a specialized Gradle source set `thirdpartylibraries` for 3rd party library source files and `thirdpartyres` for 3rd party resource files in the `main` directory.
- Create a `:repo` subfolder in the `thirdpartyres` folder and copy the resource contents from the library module from the downloaded project zip file into the new subfolder.
- Copy the contents of the `com.blueiobase.api.android.:repo` package from the downloaded project zip file into the `thirdpartylibraries` source set.
- Again, this method makes the source code accessible. If you do make major or minor improvements to the source code, consider making a pull request or an issue to make a contribution.

Check the [Contributing](https://github.com/IODevBlue/:repo/blob/development/CONTRIBUTING.md) for more information.



Usage
-----

Java Interoperability (Optional: For Kotlin projects)
---------------------

Configurations: (Optional)
---------------
|Variable |Default |Use |
|:---|:---:|:---:|
|`varName` |Default Value |Use (as in documentation). |

|Method |Returns |Use |
|:---|:---:|:---:|

XML attributes: (Optional)
--------------
|Attribute |Default |Use |
|:---|:---:|:---:|
|`varName` |Default Value |Use (as in documentation). |

Applications using :repo (Optional)
------------------------
If your application uses :repo and you'd love to showcase, send an <a href="mailto:iodevblue@gmail.com">email</a> containing:
- An app icon
- A link to download your application.
- A related Github repository.

Contributions
-------------
Contributors are welcome!

**NOTE:** This repository is split into two branches:
- [main](https://github.com/IODevBlue/:repo/tree/main) branch
- [development](https://github.com/IODevBlue/:repo/tree/development) branch

All developing implementations and proposed changes are pushed to the [development](https://github.com/IODevBlue/:repo/tree/development) branch and finalized updates are pushed to the [main](https://github.com/IODevBlue/:repo/tree/main) branch.

To note if current developments are being made, there would be more commits in the [development](https://github.com/IODevBlue/:repo/tree/development) branch than in the [main](https://github.com/IODevBlue/:repo/tree/main) branch.


Check the [Contributing](https://github.com/IODevBlue/:repo/blob/development/CONTRIBUTING.md) for more information.


Changelog
---------
* **1.0.0**
    * Initial release

More version history can be gotten from the [Change log](https://github.com/IODevBlue/:repo/blob/main/CHANGELOG.md) file.


License
=======
```
    Copyright 2023 IO DevBlue

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