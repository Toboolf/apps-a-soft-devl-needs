# Application installation guide for software developers

This is a guide for the general apps and command-line tools that are required for the _EBC_ software developers in order to develop, design, create, support (and so further) the _EBC_ applications.

## Index

#### From AppStore [](#app-store)

* [XCode](#xcode)
* [Trello](#trello)

#### From Web Page [>>](#web-page)
* [The Unarchiver](#the-unarchiver)
* [iTerm 2](#iterm)
* [Slack](#slack)
* [MacDown](#mac-down)
* [iTerm 2](#iterm)
* [iTerm 2](#iterm)

#### Via CLI [>>](#cli)
* [XCode Command Line Tools](#xcode-cli)
* [Brew](#brew)
* [Zsh](#zsh)
* [On my Zsh!](#oh-my-zsh)
* [SdkMan!](#sdkman)

#### Via SdkMan [>>](#via-sdkman)
* [Gradle](#gradle)
* [Groovy](#groovy)
* [Groovy Serv](#groovy-serv)
* [Maven](#maven)
* [Kotlin](#kotlin)
* [Scala](#scala)
* [Micronaut](#micronaut)
* [Spring Boot](#spring-boot)
* [Grails](#grails)
* [Vert.x](#vertx)

#### Via Brew [>>](#via-brew)
* [Gradle](#gradle)

#### SSH Configuration [>>](#ssh)

<br/>

# <a name="app-store"></a> From AppStore 

## <a name="xcode"></a> XCode

Includes almost everything developers need to create applications for MacOS- [AppStore](https://itunes.apple.com/mx/app/xcode/id497799835?mt=12)

#### Installation

1. Download from AppStore (requires active apple account)
2. Once installed open the XCode App and accept the terms of use
3. It will start to install some components

## <a name="trello"></a> Trello

Workspaces for project administration  - [AppStore](https://itunes.apple.com/mx/app/trello/id1278508951?mt=12)

#### Installation

1. Download from AppStore (requires active apple account)

<br/>

# <a name="web-page"></a> From Web Page

## <a name="the-unarchiver"></a> The Unarchiver

Appliaction to open RAR on MacOS - [theunarchiver.com](https://theunarchiver.com/)

#### Installation

1. Download TheUnarchiver.zip from the page
2. Unzip
2. Move TheUnarchiver.app to `~/Applications/` folder

## <a name="iterm"></a> iTerm 2

Terminal emulator for MacOS - [iterm2.com](https://www.iterm2.com/)

#### Installation

1. Download app from the page
2. Move iTerm to `~/Applications/` folder

## <a name="mac-down"></a> MacDown

MarkDown Live Editor - [macdown.uranusjr.com](https://macdown.uranusjr.com/)

#### Installation

1. Download app from the page
2. UnZip
2. Move MacDown to `~/Applications/` folder

## <a name="slack"></a> Slack

App for team colaboration - [slack.com](https://slack.com)

#### Installation

1. Download app from the [page](https://slack.com/intl/es-mx/downloads/mac)
2. Move Slack to `~/Applications/` folder

## <a name="soapui"></a> SoapUI

REST & SOAP Testing Tool - [soapui.org](https://www.soapui.org/)

#### Installation

1. Download app from the [page](https://www.soapui.org/downloads/thank-you-for-downloading-soapui.html)
2. Exec downloaded file and follow instructions

## <a name="intellij"></a> IntelliJ IDEA

IDE for Java, Groovy, Kotlin and more - [jetbrains.com](https://www.jetbrains.com/idea/)

#### Installation

1. Download app from the [page](https://www.jetbrains.com/idea/download/#section=mac)
2. Exec downloaded DMG and follow instructions

## <a name="postman"></a> Postman

API Development Environment - [getpostman.com](https://www.getpostman.com/)

#### Installation

1. Download app from the [page](https://www.getpostman.com/downloads/)
2. UnZip
3. Exec

## <a name="sql-developer"></a> SQL Developer

Database Manager ans Script execution - [oracle.com](https://www.oracle.com/technetwork/developer-tools/sql-developer/downloads/index.html)

#### Installation

1. Download app from the [page](https://www.oracle.com/technetwork/developer-tools/sql-developer/downloads/index.html)
2. Oracle account is required
3. UnZip
4. Move Sql Developer app to Application Folder

<br/>

# <a name="cli"></a> Via CLI

## <a name="xcode-cli"></a> XCode Command Line Tools

Several command line tools for developers - [developer.apple.com](https://developer.apple.com/download/more/?=command%20line%20tools)

#### Installation

##### Installing from CLI

1. From shell

	```shell
	xcode-select --install
	```
2. You will be prompted to accept terms and conditions
3. Components will start to download

	
##### Installing via web dmg download

1. Access the download page [here](https://developer.apple.com/download/more/?=command%20line%20tools)
2. An apple developer account is required
3. Select the version needed for you iMac and version of XCode (you can check the version openning XCode and in the top menu XCode > About XCode) ans download
4. Exec Command_Line_Tools.dmg
5. Double click Command Line Tools.pkg
6. Follow instructions and accept terms and conditions

## <a name="brew"></a> Brew (Homebrew)

Gestor de paquetes para MacOS - [brew.sh](https://brew.sh)

#### Installation

1. Exec the following command 

```shell
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
2. Move iTerm to `~/Applications/` folder

## <a name="zsh"></a> Zsh

* Web page: [github.com](https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH)

#### Installation

1. Run the following command

	```shell
	brew install zsh zsh-completions
	```
2. To set Zsh as default shell run:

	```shell
	chsh -s /bin/zsh
	```

## <a name="oh-my-zsh"></a> Oh my zsh !

* Web page: [ohmyz.sh](https://ohmyz.sh/)

#### Installation

1. Via curl:

	```shell
	sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
	```
	
## <a name="sdkman"></a> SdkMan!

Software Developer Kit Manager - [sdkman.io](https://sdkman.io/)

#### Installation

1. Via curl:

	```shell
	curl -s "https://get.sdkman.io" | bash
	```
2. Reaload source for the changes to take effect

	```shell
	source "$HOME/.sdkman/bin/sdkman-init.sh"
	```
3. Check if averything went well:

	```shell
	sdk version
	```
	
<br/>

# <a name="via-sdkman"></a> Via SdkMan
	
## <a name="gradle"></a> Gradle

Gradle is an open-source build automation tool focused on flexibility and performance - [gradle.org](https://gradle.org/)

#### Installation

1. Via sdkman:

	```shell
	sdk install gradle
	```
	
## <a name="groovy"></a> Groovy

Groovy is a powerful, optionally typed and dynamic language, with static-typing and static compilation capabilities, for the Java platform - [groovy-lang.org](http://groovy-lang.org/)

#### Installation

1. Via sdkman:

	```shell
	sdk install groovy
	```

## <a name="groovy-serv"></a> GroovyServ

GroovyServ reduces startup time of the JVM for runnning Groovy significantly - [github.io](https://kobo.github.io/groovyserv/)

#### Installation

1. Via sdkman:

	```shell
	sdk install groovy
	```
	
## <a name="maven"></a> Maven

Apache Maven is a software project management and comprehension tool - [maven.apache.org](https://maven.apache.org/)

#### Installation

1. Via sdkman:

	```shell
	sdk install maven
	```
	
## <a name="kotlin"></a> Kotlin

Kotlin is a statically-typed programming language that runs on the Java Virtual
Machine and can also be compiled to JavaScript source code - [kotlinlang-org](https://kotlinlang.org/)

#### Installation

1. Via sdkman:

	```shell
	sdk install kotlin
	```

## <a name="scala"></a> Scala

Scala is a programming language for general software applications - [scala-lang.org](http://www.scala-lang.org/)

#### Installation

1. Via sdkman:

	```shell
	sdk install scala
	```
	
## <a name="micronaut"></a> Micronaut

Micronaut is an open source microservice framework for the JVM - [micronaut.io](http://micronaut.io/)

#### Installation

1. Via sdkman:

	```shell
	sdk install micronaut
	```
	
## <a name="spring-boot"></a> Spring Boot 2

Spring Boot takes an opinionated view of building production-ready Spring
applications - [projects.spring.io](http://projects.spring.io/spring-boot/)

#### Installation

1. Via sdkman:

	```shell
	sdk install springboot
	```
	
## <a name="grails"></a> Grails

Grails is a powerful web framework, for the Java platform - [grails.org](https://grails.org/)

#### Installation

1. Via sdkman:

	```shell
	sdk install grails 2.5.6
	```

## <a name="vertx"></a> Vert.x

Vert.x is a tool-kit for building reactive applications on the JVM - [vertx.io](http://vertx.io/)

#### Installation

1. Via sdkman:

	```shell
	sdk install vertx
	```

<br/>

# <a name="ssh"></a> SSH Configuration

The following steps are intended to create a new pair of keys and add them, to the agent in order to start it automatically and not enter out password every time we need to use SSH.

### Step 1. Create new pair of keys

1. From the terminal, enter ssh-keygen at the command line.  
The command prompts you for a file to save the key in:

	```shell
	$ ssh-keygen 
	Generating public/private rsa key pair.
	Enter file in which to save the key (/Users/emmap1/.ssh/id_rsa):
	```

2. Press the Enter or Return key to accept the default location.
3. Enter and re-enter a passphrase when prompted.  
The command creates your default identity with its public and private keys.  
The whole interaction will look similar to the following:

	```shell
	$ ssh-keygen 
	Generating public/private rsa key pair.
	Enter file in which to save the key (/Users/emmap1/.ssh/id_rsa):
	Created directory '/Users/emmap1/.ssh'.
	Enter passphrase (empty for no passphrase):
	Enter same passphrase again:
	Your identification has been saved in /Users/emmap1/.ssh/id_rsa.
	Your public key has been saved in /Users/emmap1/.ssh/id_rsa.pub.
	The key fingerprint is:
	4c:80:61:2c:00:3f:9d:dc:08:41:2e:c0:cf:b9:17:69 emmap1@myhost.local 
	The key's randomart image is:
	+--[ RSA 2048]----+
	|*o+ooo.          |
	|.+.=o+ .         |
	|. *.* o .        |
	| . = E o         |
	|    o . S        |
	|   . .           |
	|     .           |
	|                 |
	|                 |
	+-----------------+
	```

4. List the contents of ~/.ssh to view the key files.

	```shell
	$ ls ~/.ssh 
	id_rsa id_rsa.pub
```

### Step 2. Add key to de ssh-agent

If you don't want to type your password each time you use the key, you'll need to add it to the ssh-agent.

1. To start the agent, run the following:

	```shell
	eval `ssh-agent` 
	```

2. Enter ssh-add followed by the path to the private key file:

	```shell
	ssh-add -K ~/.ssh/.id_rsa

	```
	
3. So that your computer remembers your password each time it restarts, open (or create) the ~/.ssh/config file and add these lines to the file:

	```shell
	touch ~/.ssh/config
	echo "Host *" >> ~/.ssh/config
	echo "  UseKeychain yes" >> ~/.ssh/config
	```
	
### Step 3. Add public key to a service (BitBucket)

1. Copy the public key file content

	```shell
	pbcopy < ~/.ssh/id_rsa.pub
	```
	
2. Paste it to wherever you need it 
3. To verify if the connection is succesful (example)

	```shell
	ssh -T git@bitbucket.org
	```