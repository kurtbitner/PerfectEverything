# Perfect: Server-Side Swift
![Perfect logo](https://www.perfect.org/images/icon_128x128.png)

# PerfectEverything

This repository contains all of the Perfect related Swift packages as a series of sub-repositories. 

```git clone --recursive https://github.com/PerfectlySoft/PerfectEverything.git```

Cloning this repository will give you all of the examples & datasource connectors, the starter project template, PerfectLib, reference materials and the stand-alone HTTP and FastCGI servers. This is useful for one wanting to quickly get an overview of what Perfect has to offer.

All of the projects build with Swift Package Manager and as such all require Swift 3.0.

Contents:

* PerfectLib: Core library package
* PerfectDocs: API reference material for PerfectLib
* PerfectTemplate: Simple "Hello, world!" project template
* Datasources: MySQL, Postgres, MongoDB, Redis, SQLite
* Examples: Simple server projects built with Perfect
* PerfectServer: Stand alone HTTP and FastCGI servers

Consult the READMEs in the individual projects for further details.

Consult the [main Perfect project page](https://github.com/PerfectlySoft/Perfect) for a general overview and Quick Start guide.

## Repository Layout

We have finished refactoring Perfect to support Swift Package Manager. The Perfect project has been split up into the following repositories:

* [Perfect](https://github.com/PerfectlySoft/Perfect) - This repository contains the core PerfectLib and will continue to be the main landing point for the project.
* [PerfectTemplate](https://github.com/PerfectlySoft/PerfectTemplate) - A simple starter project which compiles with SPM into a stand-alone executable HTTP server. This repository is ideal for starting on your own Perfect based project.
* [PerfectDocs](https://github.com/PerfectlySoft/PerfectDocs) - Contains all API reference related material.
* [PerfectExamples](https://github.com/PerfectlySoft/PerfectExamples) - All the Perfect example projects and documentation.
* [PerfectEverything](https://github.com/PerfectlySoft/PerfectEverything) - This umbrella repository allows one to pull in all the related Perfect modules in one go, including the servers, examples, database connectors and documentation. This is a great place to start for people wishing to get up to speed with Perfect.
* [PerfectServer](https://github.com/PerfectlySoft/PerfectServer) - Contains the PerfectServer variants, including the stand-alone HTTP and FastCGI servers. Those wishing to do a manual deployment should clone and build from this repository.
* [Perfect-Redis](https://github.com/PerfectlySoft/Perfect-Redis) - Redis database connector.
* [Perfect-SQLite](https://github.com/PerfectlySoft/Perfect-SQLite) - SQLite3 database connector.
* [Perfect-PostgreSQL](https://github.com/PerfectlySoft/Perfect-PostgreSQL) - PostgreSQL database connector.
* [Perfect-MySQL](https://github.com/PerfectlySoft/Perfect-MySQL) - MySQL database connector.
* [Perfect-MongoDB](https://github.com/PerfectlySoft/Perfect-MongoDB) - MongoDB database connector.
* [Perfect-FastCGI-Apache2.4](https://github.com/PerfectlySoft/Perfect-FastCGI-Apache2.4) - Apache 2.4 FastCGI module; required for the Perfect FastCGI server variant.

The database connectors are all stand-alone and can be used outside of the Perfect framework and server.

## Further Information
For more information on the Perfect project, please visit [perfect.org](http://perfect.org).
