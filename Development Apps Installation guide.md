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
* [SoapUI](#soapui)
* [IntelliJ IDEA](#intellij)
* [Postman](#postman)
* [SQL Developer](#sql-developer)
* [Visual Studio Code](#vs-code)
* [Opera](#opera)
* [Gatlin](#Gatlin)
* [iReports](#ireports)

#### Via CLI [>>](#cli)
* [XCode Command Line Tools](#xcode-cli)
* [Brew](#brew)
* [Zsh](#zsh)
* [On my Zsh!](#oh-my-zsh)
* [SdkMan!](#sdkman)
* [Node Version Manager - NVM](#nvm)
* [Bower](#bower)
* [Vim Plugins](#vim)

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
* [Yarn](#yarn)
* [HTTPie](#httpie)
* [BlueUtil](#blueutil)
* [jEnv](#jenv)
* [Tmux](#tmux)
* [Git-Extras](#git-extras)
* [Dockjer](#docker)
* [asdf-vm](#asdf)

#### Via asdf [>>](#via-asdf)

* [Erlang](#erlang)
* [Elixir](#elixir)

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

## <a name="vs-code"></a> Visual Studio Code

Visual Studio Code is a lightweight but powerful source code editor which runs on your desktop and is available for Windows, macOS and Linux. It comes with built-in support for JavaScript, TypeScript and Node.js and has a rich ecosystem of extensions for other languages (such as C++, C#, Java, Python, PHP, Go) and runtimes (such as .NET and Unity) - [visualstudio.com](https://code.visualstudio.com/)

#### Installation

1. Download app from the [page](https://code.visualstudio.com/docs/?dv=osx)
2. UnZip
3. Move Visual Studio Code app to Application Folder

## <a name="opera"></a> Opera

Navegador con VPN gratuita, bloqueador de publicidad rápido, soporte Web 3, control de experiencia de navegación - [opera.com](https://www.opera.com/es-419)

#### Installation

1. Download app from the [page](https://www.opera.com/es-419/computer/thanks?ni=stable&os=mac)
2. UnZip
3. Exec installer
4. Follow instructions

## <a name="gatlin"></a> Gatlin

Gatling is a highly capable load testing tool. It is designed for ease of use, maintainability and high performance - [gatlin.io](https://gatling.io/)

#### Installation

1. Download app from the [page](https://gatling.io/download/)
2. UnZip
3. Move folder to your preferred path

## <a name="ireports"></a> iReports

Visual designer tool for JasperReports Library and JasperReports Server (Business Intelligence) - [community.jaspersoft.com](https://community.jaspersoft.com/project/ireport-designer)

#### Installation

1. Download app from the [page](https://sourceforge.net/projects/ireport/)
2. Exec dmg
3. Move Jaspersoft iReport Designer app to `~/Applcations` folder
4. Path to JDK 7 must be set in the App conf, run the following command, the path must be to your own jdk 7:

	```shell
	echo 'jdkhome="/Library/Java/JavaVirtualMachines/jdk1.7.0_80.jdk/Contents/Home"' >> /Applications/Jaspersoft\ iReport\ Designer.app/Contents/Resources/ireport/etc/ireport.conf
	```

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
	
## <a name="nvm"></a> NVM

Node Version Manager - [github.io](https://github.com/nvm-sh/nvm)

#### Installation

1. Via curl:

	```shell
	curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
	```
2. Add the following lines to your `.zshrc` file:

	```shell
	export NVM_DIR="$HOME/.nvm"
	[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
	[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
	```
	
	You can use the following to automatically add them:
	
	```shell
	echo 'export NVM_DIR="$HOME/.nvm"' >> ~/.zshrc
	echo '[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"' >> ~/.zshrc
	echo '[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"' >> ~/.zshrc
	```
3. Reopen the terminal or:

	```shell
	source ~/.zshrc
	```

4.	Install the most recent version of node:

	```shell
	nvm install node
	```
	
## <a name="bower"></a> Bower

A package manager for the web - [bower.io](https://bower.io/)

#### Installation

1. Via npm:

	```shell
	npm install -g bower
	```
	
## <a name="vim"></a> Vim Plugins

Plugins for vim - [sohjiro/.vim](https://github.com/sohjiro/.vim)

#### Installation

1. Via curl:

	```shell
	curl -L https://raw.githubusercontent.com/sohjiro/.vim/master/run_config.sh | sh
	```
2. Open ´vim´ and run the following command:

	```shell
	:PlugInstall
	```
3. Reopne terminal
	
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

# <a name="via-brew"></a> Via Brew

## <a name="yarn"></a> Yarn

Yarn is a package manager for your code. It allows you to use and share code with other developers from around the world - [yarnpkg.com](https://yarnpkg.com)

#### Installation

1. Via Brew:

	```shell
	brew install yarn
	```
	
## <a name="httpie"></a> HTTPie

HTTPie—aitch-tee-tee-pie—is a command line HTTP client with an intuitive UI, JSON support, syntax highlighting, wget-like downloads, plugins, and more - [httpie.org](https://httpie.org/)

#### Installation

1. Via Brew:

	```shell
	brew install httpie
	```

## <a name="blueutil"></a> blueutil

CLI for bluetooth on OSX: power, discoverable state, list, inquire devices, connect, info - [github.com/toy](https://github.com/toy/blueutil)

#### Installation

1. Via Brew:

	```shell
	brew install blueutil
	```

## <a name="jenv"></a> jEnv

jEnv is a command line tool to help you forget how to set the JAVA_HOME environment variable - [jenv.be](https://www.jenv.be/)

#### Installation

1. Via Brew:

	```shell
	brew install jenv
	```
2. Add the following lines to the end of `.zshrc` file:

	```shell
	export PATH="$HOME/.jenv/bin:$PATH"
	eval "$(jenv init -)"
	```
	You can exec this directly but be carefull with the SDKMAN config:
	
	```shell
	echo 'export PATH="$HOME/.jenv/bin:$PATH"' >> ~/.zshrc
	echo 'eval "$(jenv init -)"' >> ~/.zshrc
	```
3. Add your downloaded JDK like so:

	```shell
	jenv add /System/Library/Java/JavaVirtualMachines/1.6.0.jdk/Contents/Home
	jenv add /Library/Java/JavaVirtualMachines/jdk17011.jdk/Contents/Home
	```
	
## <a name="tmux"></a> Tmux

Terminal multiplexer - [tmux](https://github.com/tmux/tmux/wiki)

#### Installation

1. Via Brew:

	```shell
	brew install tmux
	```
2. Create tmux config file:

	```shell
	touch ~/.tmux.conf
	```
3. Exec the following command to add lines to `~/.tmux.conf`:

	```shell
	cat >> ~/.tmux.conf <<EOL
	#option -g default-command "reattach-to-user-namespace -l zsh"
	set -g prefix C-a
	unbind C-b
	set -sg escape-time 1
	set -g base-index 1
	setw -g pane-base-index 1
	bind r source-file ~/.tmux.conf \; display "Configuración recargada"
	bind C-a send-prefix
	bind | split-window -h -c "#{pane_current_path}"
	bind - split-window -v -c "#{pane_current_path}"
	bind c new-window -c "#{pane_current_path}"
	bind h select-pane -L
	bind j select-pane -D
	bind k select-pane -U
	bind l select-pane -R
	bind -r C-h select-window -t :-
	bind -r C-l select-window -t :+
	bind -r H resize-pane -L 5
	bind -r J resize-pane -D 5
	bind -r K resize-pane -U 6
	bind -r L resize-pane -R 5
	setw -g mode-mouse off
	set -g mouse-select-pane off
	set -g mouse-resize-pane off
	#set mouse-select-window off
	set -g default-terminal "screen-256color"
	set -g status-fg white
	set -g status-bg black
	setw -g window-status-fg cyan
	setw -g window-status-bg default
	setw -g window-status-attr dim
	setw -g window-status-current-fg white
	setw -g window-status-current-bg red
	setw -g window-status-current-attr bright
	set -g pane-border-fg green
	set -g pane-border-bg black
	set -g pane-active-border-fg white
	set -g pane-active-border-bg yellow
	set -g message-fg white
	set -g message-bg black
	set -g message-attr bright
	set -g status-left-length 40
	set -g status-left "#[fg=green]Session: #S #[fg=yellow]#I #[fg=cyan]#P"
	set -g status-right "#[fg=cyan]%d %b %R"
	setw -g utf8 on
	set -g status-utf8 on
	set -g status-interval 60
	set -g status-justify centre
	setw -g monitor-activity on
	set -g visual-activity on
	setw -g mode-keys vi
	unbind [
	bind Escape copy-mode
	unbind p
	bind p paste-buffer
	bind -t vi-copy 'v' begin-selection
	bind -t vi-copy 'y' copy-selection
	bind -n C-k send-keys -R \; clear-history
	EOL
	```
		
## <a name="git-extras"></a> Git Extras

Little git extras - [tj/git-extras](https://github.com/tj/git-extras)

#### Installation

1. Via Brew:

	```shell
	brew install git-extras
	```
	
## <a name="docker"></a> Docker

Enterprise Container Platform for High-Velocity Innovation - [docker.com](https://www.docker.com/)

#### Installation

1. Via Brew:

	```shell
	brew cask install docker
	```
2. Install docker

	```shell
	brew install docker
	brew install docker-completion
	```
	
3. Install docker-machine

	```shell
	brew install docker-machine
	```

## <a name="asdf"></a> asdf-vm

Manage multiple runtime versions with a single CLI tool - [asdf-vm.com](https://asdf-vm.com/#/)

#### Installation

1. Via Brew:

	```shell
	brew install asdf
	```
	
2. Add the following lines to the `.zshrc` file:

	```shell
	. /usr/local/opt/asdf/asdf.sh
	. /usr/local/opt/asdf/etc/bash_completion.d/asdf.bash
	```
	
	Or for automatically do it(be carefull with sdkman config):
	
	```shell
	echo -e '\n. /usr/local/opt/asdf/asdf.sh' >> ~/.zshrc
	echo -e '\n. /usr/local/opt/asdf/etc/bash_completion.d/asdf.bash' >> ~/.zshrc
	```
	
3. Install plugin common dependencies:

	```shell
	brew install \
	  coreutils automake autoconf openssl \
	  libyaml readline libxslt libtool unixodbc \
	  unzip curl
	```
	
## <a name="siege"></a> Siege

Siege is an http load testing and benchmarking utility - [joedog.org](https://www.joedog.org/siege-home/)

#### Installation

1. Via Brew:

	```shell
	brew install siege
	```
	
## <a name="postgresql"></a> PostgreSQL

PostgreSQL is a powerful, open source object-relational database  - [postgresql.org](https://www.postgresql.org/)

#### Installation

1. Via Brew:

	```shell
	brew install postgresql
	ln -sfv /usr/local/opt/postgresql/*.plist ~/Library/LaunchAgents
	```
2. Add alias to `.zshrc`:

	```shell
	alias pg_start="launchctl load ~/Library/LaunchAgents/homebrew.mxcl.postgresql.plist"
	alias pg_stop="launchctl unload ~/Library/LaunchAgents/homebrew.mxcl.postgresql.plist"
	```
	
	Or run the following commands(be careful with the SDKMAN config):
	
	```shell
	echo 'alias pg_start="launchctl load ~/Library/LaunchAgents/homebrew.mxcl.postgresql.plist"' >> ~/.zshrc
	echo 'alias pg_stop="launchctl unload ~/Library/LaunchAgents/homebrew.mxcl.postgresql.plist"' >> ~/.zshrc
	```
	
3. Config PostgreSQL

	```shell
	source ~/.zshrc
	pg_start
	createdb `whoami`
	pg_stop
	```

<br/>

# <a name="via-asdf"></a> Via asdf

## <a name="erlang"></a> Erlang

Erlang is a programming language used to build massively scalable soft real-time systems with requirements on high availability - [erlang.org](https://www.erlang.org/)

#### Installation

1. Via asdf:

	```shell
	asdf plugin-add erlang
	asdf install erlang 22.0.2
	asdf global erlang 22.0.2
	```

## <a name="elixir"></a> Elixir

Elixir is a dynamic, functional language designed for building scalable and maintainable applications - [elixir-lang.org](https://elixir-lang.org/)

#### Installation

1. Via asdf:

	```shell
	asdf plugin-add elixir
	asdf install elixir 1.8.2
	asdf global elixir 1.8.2
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