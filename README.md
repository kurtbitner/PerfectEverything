# Perfect: Server-Side Swift
![Perfect logo](https://www.perfect.org/images/icon_128x128.png)

[![Swift 2.2](https://img.shields.io/badge/Swift-2.2-orange.svg?style=flat)](https://developer.apple.com/swift/)
[![Swift 3.0](https://img.shields.io/badge/Swift-3.0-orange.svg?style=flat)](https://developer.apple.com/swift/)
[![Platforms OS X | Linux](https://img.shields.io/badge/Platforms-OS%20X%20%7C%20Linux%20-lightgray.svg?style=flat)](https://developer.apple.com/swift/)
[![License Apache](https://img.shields.io/badge/License-Apache-lightgrey.svg?style=flat)](http://perfect.org/licensing.html)
[![Docs](https://img.shields.io/badge/docs-83%-yellow.svg?style=flat)](http://www.perfect.org/docs/)
[![Issues](https://img.shields.io/github/release/qubyte/rubidium.svg)](https://github.com/PerfectlySoft/Perfect/issues)
[![Donate](https://img.shields.io/badge/Donate-PayPal-blue.svg?style=flat)](https://paypal.me/perfectlysoft)
[![Twitter](https://img.shields.io/badge/Twitter-@PerfectlySoft-brightgreen.svg?style=flat)](http://twitter.com/PerfectlySoft)
[![Join the chat at https://gitter.im/PerfectlySoft/Perfect](https://img.shields.io/badge/Gitter-Join%20Chat-brightgreen.svg)](https://gitter.im/PerfectlySoft/Perfect?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

**The master branch of this project currently compiles with Swift 2.2 and with the 3.0-dev MAY toolchain using Swift Package Manager.**

# PerfectStarter

This repository contains all the modules as a series of sub-repositories. This gives you PerfectLib & PerfectServer, as well as every database connector and example.

```git clone --recursive https://github.com/PerfectlySoft/PerfectStarter.git```

Perfect is an application server for Linux or OS X which provides a framework for developing web and other REST services in the Swift programming language. Its primary focus is on facilitating mobile apps which require backend server software, enabling you to use one language for both front and back ends.

Perfect operates using either its own stand-alone HTTP/HTTPS server or through FastCGI. It provides a system for loading your own Swift based modules at startup and for interfacing those modules with its request/response objects or to the built-in mustache template processing system.

Perfect is built on its own high performance completely asynchronous networking engine with the goal of providing a scalable option for internet services. It supports SSL out of the box and provides a suite of tools which are commonly required by internet servers, such as WebSockets and iOS push notifications, but does not limit your options. Feel free to swap in your own favorite JSON or templating systems, etc.

## Quick Start

### OS X
Perfect relies on [Home Brew](http://brew.sh) for installing dependencies on OS X. This is currently limited to OpenSSL. To install Home Brew:

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

To install OpenSSL:

```
brew install openssl
brew link openssl --force
```

### Linux
Perfect relies on libcurl and OpenSSL:

```
sudo apt-get install libcurl-dev openssl
```

### Build Starter Project

The following will clone and build an empty starter project and launch the server on port 8181.

```
git clone https://github.com/PerfectlySoft/PerfectTemplate.git
cd PerfectTemplate
swift build
.build/debug/PerfectTemplate
```

Access [localhost:8181](http://127.0.0.1:8181/) to see the greeting. See the full source code for [PerfectTemplate](https://github.com/PerfectlySoft/PerfectTemplate).

## Repository Layout

We have finished refactoring Perfect to support Swift Package Manager. The Perfect project has been split up into the following repositories:

* [Perfect](https://github.com/PerfectlySoft/Perfect) - This repository contains the core PerfectLib and will continue to be the main landing point for the project.
* [PerfectTemplate](https://github.com/PerfectlySoft/PerfectTemplate) - A simple starter project which compiles with SPM into a stand-alone executable HTTP server. This repository is ideal for starting on your own Perfect based project.
* [PerfectStarter](https://github.com/PerfectlySoft/PerfectStarter) - This umbrella repository allows one to pull in all the related Perfect modules in one go, including the servers, examples, database connectors and documentation. This is a great place to start for people wishing to get up to speed with Perfect.
* [PerfectDocs](https://github.com/PerfectlySoft/PerfectDocs) - Contains all API reference related material.
* [PerfectExamples](https://github.com/PerfectlySoft/PerfectExamples) - All the Perfect example projects and documentation.
* [PerfectServer](https://github.com/PerfectlySoft/PerfectServer) - Contains the PerfectServer variants, including the stand-alone HTTP and FastCGI servers. Those wishing to do a manual deployment should clone and build from this repository.
* [Perfect-FastCGI-Apache2.4](https://github.com/PerfectlySoft/Perfect-FastCGI-Apache2.4) - Apache 2.4 FastCGI module; required for the Perfect FastCGI server variant.
* [Perfect-SQLite](https://github.com/PerfectlySoft/Perfect-SQLite) - SQLite3 database connector.
* [Perfect-PostgreSQL](https://github.com/PerfectlySoft/Perfect-PostgreSQL) - PostgreSQL database connector.
* [Perfect-MySQL](https://github.com/PerfectlySoft/Perfect-MySQL) - MySQL database connector.
* [Perfect-MongoDB](https://github.com/PerfectlySoft/Perfect-MongoDB) - MongoDB database connector.

The database connectors are all stand-alone and can be used outside of the Perfect framework and server.

## Further Information
For more information on the Perfect project, please visit [perfect.org](http://perfect.org).
