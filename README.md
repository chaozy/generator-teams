# Microsoft Teams App Project Generator - #YoTeams

[![npm version](https://badge.fury.io/js/generator-teams.svg)](https://www.npmjs.com/package/generator-teams)
[![npm](https://img.shields.io/npm/dt/generator-teams.svg)](https://www.npmjs.com/package/generator-teams)
[![MIT](https://img.shields.io/npm/l/generator-teams.svg)](https://github.com/PnP/generator-teams/blob/master/LICENSE.md)
[![GitHub issues](https://img.shields.io/github/issues/PnP/generator-teams.svg)](https://github.com/PnP/generator-teams/issues)
[![GitHub closed issues](https://img.shields.io/github/issues-closed/PnP/generator-teams.svg)](https://github.com/PnP/generator-teams/issues?q=is%3Aissue+is%3Aclosed)
[![GitHub stars](https://img.shields.io/github/stars/PnP/generator-teams.svg)](https://github.com/PnP/generator-teams/stargazers)
[![Gitter](https://badges.gitter.im/PnP/generator-teams.svg)](https://gitter.im/OfficeDev/generator-teams?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

 | @master | @preview |
 :--------:|:---------:
 [![npm (latest)](https://img.shields.io/npm/v/generator-teams/latest.svg)](https://www.npmjs.com/package/generator-teams)|[![npm (preview)](https://img.shields.io/npm/v/generator-teams/preview.svg)](https://www.npmjs.com/package/generator-teams)
 [![Travis (.org) branch](https://img.shields.io/travis/PnP/generator-teams/master.svg)](https://travis-ci.org/PnP/generator-teams)|[![Travis (.org) branch](https://img.shields.io/travis/PnP/generator-teams/preview.svg)](https://travis-ci.org/PnP/generator-teams)

A [Yeoman Generator](http://yeoman.io/) for [Microsoft Teams](https://teams.microsoft.com) Apps projects. **The most comprehensive and complete development toolkit for Microsoft Teams development**. This generator is for developers who prefers to use TypeScript, React and node as their primary technologies.

The generator allows you to simply create and scaffold projects that includes one or more Microsoft Teams features such as:

* Bots - based on Bot Framework
* Messaging Extensions - actions and query
* Tabs, with support for Single-Sign-On
* Connectors
* Outgoing Webhooks

When scaffolding the project you will also have the option of adding additional features to your project such as:

* Easy deploy to Microsoft Azure
* Add unit testing framework and sample unit tests
* Easily develop and debug using ngrok
* Application Insights support

## Documentation

The documentation for the generator and the generated project can be found at the [generator-teams Github Wiki](https://github.com/PnP/generator-teams/wiki).

## The generated project

When the generator is done you can start working with your project. Make sure to read the generated README.md file for more instructions. The generated artefacts contain sample code as well as detailed documentation on the required steps that is required for you when registering Connectors and Bots.

The solution can be built using the Gulp task `build` and hosted on a local web server using the Gulp task `serve`. The Teams Application manifest is generated by executing the Gulp task `manifest` - that will validate and create the ZIP file that you upload to Microsoft Teams.

## yo teams Demo

![Demo](docs/assets/demo.gif)

## Install

> **Important:** If this is the first time you're using Yeoman or installing a Yeoman generator, first install [Node.js](https://nodejs.org). For developers on Mac, we recommend using [Node Version Manager](https://github.com/creationix/nvm) to install Node.js with the right permissions. When the installation completes, restart your console (or if you are using Windows, restart your machine) to ensure you use the updated system environment variables.

### Prerequisites

Install `yo` (Yeoman), `gulp-cli` (Gulp global command line interface) and `typescript` (Typescript compiler) globally using NPM.

``` Shell
npm install yo gulp-cli typescript --global
```


### Released and stable version

Install `generator-teams` globally using NPM.

```Shell
npm install generator-teams --global
```

### Preview versions

Preview versions of the generator will be published with the **preview** tag and can be installed using the following command:

``` Shell
npm install generator-teams@preview --global
```

## Usage

``` Shell
yo teams [arguments]
```

> *Note:* Files are created in the directory that you run the command from hence make sure you are happy with the location before you hit enter.

### Arguments

 The following arguments can be used:

* `--skip-install` - when used no packages will be installed at the end of the generator and you have to run `npm install` or similar manually.
* `--no-telemetry` - opt out of sending telemetry data (NOTE: no personal data or names of artefacts are being sent, only information of successful executions and what options are being used).

## Build the generator

If you are interested in contributing or modifying the generator itself, you clone this repository and then install all modules before building the solution.

``` Shell
npm install
npm run build
```

The bundled generator and the template files will end up in the `./generators/` folder.

## Test the generator

If you want to run the generator tests, you can run the following command.

``` Shell
npm test
```

Yeoman-test package is being used for the generator tests. (NOTE: Node JS version 8.10.0 is recommended for executing generator tests.)

### Use it in dev mode

In the `generator-teams` directory use the following command, this will link the local copy of the folder as a global node module.

``` Shell
npm link
```

To revert the link operation:

``` Shell
npm unlink
```

## More information

For more information on how Tabs and Bots can be used with Teams see the [Teams Developer Documentation](https://msdn.microsoft.com/en-us/microsoft-teams/ )

## Contributors & Hall of fame

* [Wictor Wilén](https://github.com/wictorwilen) - Original author and coordinator
* [Bill Bliss](https://github.com/billbliss)
* [Richard DiZerega](https://github.com/richdizz)
* [Elaine van Bergen](https://github.com/laneyvb)
* [Daniel Laskewitz](https://github.com/Laskewitz)
* [Paul Schaeflein](https://github.com/pschaeflein)
* [Cagdas Davulcu](https://github.com/cagdasdavulcu)
* [Stefan Bauer](https://github.com/StfBauer)
* [Andrew Connell](https://github.com/andrewconnell)
* [Ralf Brennscheidt](https://github.com/RalfBrennscheidt)
* [Felipe Plets](https://github.com/felipeplets)
* [Brendan Andrade](https://github.com/BrendanAndrade)
* [Jason Merino](https://github.com/jasonmerino)
* [Orta Therox](https://github.com/orta)
* [Oleksandr Fediashov](https://github.com/layershifter)

## Be a part of the movement

If you want to be a part of the #YoTeams movement then head on over to the discussion at the [generator-teams Gitter channel](https://gitter.im/PnP/generator-teams) or follow us on [Twitter using the hashtag #yoteams](https://twitter.com/search?q=%23yoteams&src=typd).

## Contributing

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
