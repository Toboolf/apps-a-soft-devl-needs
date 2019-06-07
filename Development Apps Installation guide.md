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
* [On my Zsh!](#oh-my-zsh)
* [Brew](#brew)
* [The Unarchiver](#the-unarchiver)
* [The Unarchiver](#the-unarchiver)
* [The Unarchiver](#the-unarchiver)
* [The Unarchiver](#the-unarchiver)
* [The Unarchiver](#the-unarchiver)
* [The Unarchiver](#the-unarchiver)

#### SSH Configuration [>>](#ssh)

<br/>

# <a name="app-store"></a> From AppStore 

## <a name="xcode"></a> XCode

Includes almost everything developers need to create applications for MacOS- [AppStore](https://itunes.apple.com/mx/app/xcode/id497799835?mt=12)

#### Installation

1. Download from AppStore (requires active apple account)

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

<br/>

# <a name="cli"></a> Via CLI

## <a name="brew"></a> Brew (Homebrew)

Gestor de paquetes para MacOS - [brew.sh](https://brew.sh)

#### Installation

1. Exec the following command 

```shell
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
2. Move iTerm to `~/Applications/` folder

## <a name="oh-my-zsh"></a> Oh my zsh !

* Web page: [ohmyz.sh](https://ohmyz.sh/)

#### Installation

1. Download app from the pageapp
2. Move iTerm to `~/Applications/` folder

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