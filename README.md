
# Arma 3 After Action Replay *Addon* Component

<a href="https://github.com/alexcroox/R3/releases/latest">
    <img src="https://img.shields.io/github/release/alexcroox/r3.svg" alt="Project Version" />
</a>    

<a href="https://github.com/alexcroox/R3/releases/latest">
    <img src="https://img.shields.io/badge/32--bit-64--bit-orange.svg" alt="Supports 64-bit" />
</a>

<a href="https://github.com/alexcroox/R3/releases/latest">
    <img src="https://img.shields.io/badge/Windows-Linux-lightgrey.svg" alt="Support for both Windows and Linux" />
</a>

<a href="https://travis-ci.org/alexcroox/R3">    
    <img src="https://travis-ci.org/alexcroox/R3.svg?branch=master&style=flat-square" alt="Travis build testing" />
</a>

<a href="https://raw.githubusercontent.com/alexcroox/R3/master/LICENSE">
    <img src="https://img.shields.io/badge/license-MIT-red.svg" alt="Project License" />
</a>

<p>
    <sup><strong>Requires the latest version of <a href="https://github.com/CBATeam/CBA_A3/releases">CBA A3</a><br/></strong></sup>
</p>

Server Side addon for capturing unit movement and behaviour to a database for After Action Replays on a website.

No modifications to your missions required, nothing for clients to download.

Being built along side the [web component](https://github.com/alexcroox/R3-Web), [extension component](https://github.com/alexcroox/R3-Extension) and the [tile generation component](https://titanmods.xyz/r3/tiler/)

Built for Windows or Linux game servers.

### Demo

An exact mirror of this repo [can be viewed here](https://aar.ark-group.org) which contains replays from [ARK Group](http://ark-group.org/)

**Note: R3 is currently undergoing a big v1 data storage refactor [read more](https://github.com/alexcroox/R3-Web/issues/14)**

<a href="https://discord.gg/qcE3dRP">
    <img width="100" src="http://i0.kym-cdn.com/photos/images/original/001/243/213/52a.png" alt="Discord">
</a>

### Install Windows Server

1. Download the [latest release](https://github.com/alexcroox/R3/releases/latest) to your Windows game server
2. Create a folder `/R3Extension/` in `/%appdata%/local/` or set environment variable `R3_EXTENSION_HOME` to a folder of your choice
3. Create a `config.properties` in the previous created folder with [this template](https://github.com/alexcroox/R3-Extension/blob/master/config.properties)
4. Create a MySQL database (on your web hosting) with [this structure](https://github.com/alexcroox/R3-Web/blob/master/db-template.sql)
5. Enter your db details into `config.properties`
6. Add @R3 to your server startup mod list
7. Host the [web component, follow instructions here](https://github.com/alexcroox/R3-Web)

### Install Linux Server

*Not yet part of the release download, see [issue #15](https://github.com/alexcroox/R3/issues/15)*

1. Download the [latest release](https://github.com/alexcroox/R3/releases/latest) to your Linux game server
2. Create a folder in the Linux user's home folder Arma will be run from at `~/R3Extension` or set environment variable `R3_EXTENSION_HOME` to a folder of your choice
3. Create a `config.properties` in the previous created folder with [this template](https://github.com/alexcroox/R3-Extension/blob/master/config.properties)
4. Create a MySQL database (on your web hosting) with [this structure](https://github.com/alexcroox/R3-Web/blob/master/db-template.sql)
5. Enter your db details into `config.properties`
6. Add @r3 to your server startup mod list (make sure it's lower case for Linux servers)
7. Host the [web component, follow instructions here](https://github.com/alexcroox/R3-Web)

### Special thanks

[ARK] Kami for building the custom db extension and allowing me to ditch extdb!

ACE3 dev team for providing [coding guidelines](http://ace3mod.com/wiki/development/coding-guidelines.html) and the [project template](https://github.com/acemod/arma-project-template) this was created from.

[ARK] Chairbourne for providing CUP source for the vehicle icons

[NRF1] Crazy for working with me on the original AAR as part of the old 5th Rifles mission framework.
