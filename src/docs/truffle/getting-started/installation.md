---
title: Truffle | Installation
layout: docs.hbs
---
# Installation

```bash
npm install -g truffle
```


## Requirements

* NodeJS v8.9.4 or later
* Windows, Linux or Mac OS X

Truffle also requires that you have a running Ethereum client which supports the standard JSON RPC API (which is nearly all of them). There are many to choose from, and some better than others for development. We'll discuss them in detail in the [Choosing an Ethereum client](/docs/getting_started/client) section.

## Recommendations for Windows

If you're running Truffle on Windows, you may encounter some naming conflicts that could prevent Truffle from executing properly. Please see [the section on resolving naming conflicts](/docs/advanced/configuration#resolving-naming-conflicts-on-windows) for solutions.


SAMPLE INSTALL
After Days of trouble trying to get clean install of Truffle, this procedure was successful.

OS: Ubuntu 20
VM: Created from fresh Ubuntu ISO

Insure your installation user has full SUDO privs.

# Verify our user is in the SUDO group.  Check by issueing:

~$ id yourUserName

Once you confirm that your user is in the SUDO group, check the SUDOERS file:

~$ sudo visudo

You should see an entry like this:

# Allow members of group sudo to execute any command
%sudo   ALL=(ALL:ALL) ALL

Once that is complete, move on to the installs


### INSTALL NVM:
### NVM option 1
~$ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash

Once complete, log out/into new terminal or issue the following to make active:

export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion

### NCM oprion 2
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash

export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion

##INSTALL NPM
~$ sudo apt install npm

## List available remote installs
## Install your preference from output

### In case you haven't done this already, do now
~$ sudo apt-get install software-properties-common
~$ sudo apt install build-essential

~$ npm update node

sudo apt update
sudo curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.35.1/install.sh | bash

export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion

nvm use 14.16.1
nvm ls
npm cache clean -f
npm install -g n

### may be helpful
apt list
apt list node
apt list nodejs

## Install latest NPM
nvm install-latest-npm

## List available remote packages
nvm ls-remote

## Choose the package you wish to activate
nvm use 14.16.1

npm install -g n
npm ls

## Install ethereum
sudo add-apt-repository -y ppa:ethereum/ethereum
sudo apt-get update
sudo apt-get install ethereum
 
## Install Truffle 
npm install -g truffle

## Deal with truffle install warnings -will vary depending on your install scenario
npm mkdirp latest
npm update mkdirp
npm install promises
npm update node-pre-gyp
npm update Debug
npm update core-js@3
npm audit

## In the end, your versions should look something like this:

~$ npm -v
7.10.0

~$ nvm version
v14.16.1

~$ node -v
v14.16.1

~$ nodejs -v
v10.19.0

~$ truffle version
Truffle v5.3.2 (core: 5.3.2)
Solidity v0.5.16 (solc-js)
Node v14.16.1
Web3.js v1.3.5

~$ geth version
Geth
Version: 1.10.2-stable
Git Commit: 97d11b0187b4695ccf44e3b71b54155fe405a36f
Architecture: amd64
Go Version: go1.16
Operating System: linux
GOPATH=
GOROOT=go
