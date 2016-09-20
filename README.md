[![Build Status](https://travis-ci.org/gorkem/vscode-java.svg?branch=master)](https://travis-ci.org/gorkem/vscode-java) [![Stories in Ready](https://badge.waffle.io/gorkem/vscode-java.png?label=ready&title=Ready)](https://waffle.io/gorkem/vscode-java)

Language support for Java &trade; for Visual Studio Code
=====================

Provides Java &trade; language support via
[java-language-server](https://github.com/gorkem/java-language-server), which utilizes
[Eclipse &trade; JDT](http://www.eclipse.org/jdt/).

Quick Start
============
1. Install the Extension
2. If you do not have a _Java 8_ Runtime on current system path or _JAVA_HOME_ is not correctly set to point to one
    * Download and install a Java 8 compatible runtime.
3. Extension is activated when you first access a Java file.
    * Initial activation can be longer since it requires extension to download additional parts.
    * Recognizes only projects with *maven* build files on the directory hierarchy. 

What is new in 0.0.3 
====================
* In addition to maven, we now support basic Eclipse projects [details](https://github.com/gorkem/java-language-server/issues/37). 
* Go to Definition (<kbd>F12</kbd>) is enabled for libraries and can display Java code that is not part of project's source code
* Code complete triggers are added for `.#@` characters. 
#### Significant bugs 
* [Opening maven project a 2nd time doesn't work](https://github.com/gorkem/java-language-server/issues/66)


Features 
=========
![ screencast ](https://raw.githubusercontent.com/gorkem/vscode-java/master/images/vscode-java.0.0.1.gif)

* Maven pom.xml project support
* As you type reporting of parsing and compilation errors
* Code completion
* Javadoc hovers 
* Code outline
* Code navigation
* Code lens (references)
* Highlights
* Code formatting

Troubleshooting
===============
1. Due to size restrictions on the marketplace extension downloads additional required parts check that they 
are downloaded under `~/.vscode/extensions/redhat.java-0.0.2/server` folder. 
You should see a folder named `plugins`.

2. Check the status of the language tools on the lower right corner (marked with A on image below).
It should show ready (thumbs up) as on the image below. You can click on the status and open the 
language tool logs for further information in case of a failure. 

![ status indicator ](https://raw.githubusercontent.com/gorkem/vscode-java/master/images/statusMarker.png)

3. Report any problems you face to the [project](https://github.com/gorkem/vscode-java/issues).

Contributing
===============
This is an open source project open to anyone. Contributions are extremely welcome 

For information on getting started refer to [java-language-server](https://github.com/gorkem/java-language-server/blob/master/README.md).

Feedback
===============
* File a bug in [GitHub Issues](https://github.com/gorkem/vscode-java/issues).
* [Tweet](https://twitter.com/GorkemErcan) us with other feedback.


License
===============
EPL 1.0, See [LICENSE](LICENSE) for more information.
