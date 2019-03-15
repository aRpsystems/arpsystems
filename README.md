<h1 align="center">
	<img
		width="300"
		alt="aRp Systems"
		src="https://raw.githubusercontent.com/arpsystems/arpsystems/master/client/img/logo-vertical-transparent-bg.svg?sanitize=true">
</h1>

<h3 align="center">
	Webchat Browser aRp Systems http://irc.arp.systems
</h3>

<p align="center">
	<strong>
		<a href="http://arp.systems/">Website</a>
		•
		<a href="http://arp.systems/docs">Docs</a>
		•
		<a href="https://demo.arp.systems/">Demo</a>
	</strong>
</p>
<p align="center">
	<a href="https://irc.arp.systems/"><img
		alt="#music IRC channel my Network"
		src="https://img.shields.io/badge/freenode-%23arpsystems-415364.svg?colorA=ff9e18&style=flat-square"></a>
	<br>
	<a href="https://yarn.pm/arpsystems"><img
		alt="npm version"
		src="https://img.shields.io/npm/v/arpsystems.svg?style=flat-square&maxAge=3600"></a>
	<a href="https://travis-ci.com/arpsystems/arpsystems"><img
		alt="Travis CI Build Status"
		src="https://img.shields.io/travis/com/arpsystems/arpsystems/master.svg?style=flat-square&maxAge=60"></a>
	<a href="https://david-dm.org/arpsystems/arpsystems"><img
		alt="Dependencies Status"
		src="https://img.shields.io/david/arpsystems/arpsystems.svg?style=flat-square&maxAge=3600"></a>
	<a href="https://npm-stat.com/charts.html?package=arpsystems&from=2016-02-12"><img
		alt="Total downloads on npm"
		src="https://img.shields.io/npm/dt/arpsystems.svg?colorB=007dc7&style=flat-square&maxAge=3600"></a>
</p>

## Overview

* **Modern features brought to IRC.** Push notifications, link previews, new message markers, and more bring IRC to the 21st century.
* **Always connected.** Remains connected to IRC servers while you are offline.
* **Cross platform.** It doesn't matter what OS you use, it just works wherever Node.js runs.
* **Responsive interface.** The client works smoothly on every desktop, smartphone and tablet.
* **Synchronized experience.** Always resume where you left off no matter what device.

To learn more about configuration, usage and features of aRp Systems, take a look at [the website](https://arp.systems).

aRp Systems is the official and community-managed fork of [Shout](https://github.com/erming/shout), by [Mattias Erming](https://github.com/erming).

## Installation and usage

aRp systems requires [Node.js](https://nodejs.org/) v6 or more recent.
[Yarn package manager](https://yarnpkg.com/) is also recommended.  
If you want to install with npm, `--unsafe-perm` is required for a correct install.

### Running stable releases using Yarn (recommended)

Run this in a terminal to install (or upgrade) the latest stable release from
[npm registry](https://www.npmjs.com/):

```sh
yarn global add arpsystems
```

If you already have aRp systems installed globally, use the following command to update it:

```sh
yarn global upgrade arpsystems
```

When installation is complete, run:

```sh
arpsystems start
```

For more information, read the [usage documentation](http://arp.systems/docs/usage) or run:

```sh
arpsystems --help
```

### Running from source

The following commands install and run the development version of The Lounge:

```sh
git clone https://github.com/arpsystems/arpsystems.git
cd arpsystems
yarn install
NODE_ENV=production yarn build
yarn start
```

When installed like this, `arpsystems` executable is not created. Use `node index <command>` to run commands.

⚠️ While it is the most recent codebase, this is not production-ready! Run at
your own risk. It is also not recommended to run this as root.

## Development setup

Simply follow the instructions to run The Lounge from source above, on your own
fork.

Before submitting any change, make sure to:

- Read the [Contributing instructions](https://github.com/arpsystems/arpsystems/blob/master/.github/CONTRIBUTING.md#contributing)
- Run `yarn test` to execute linters and test suite
- Run `yarn build` if you change or add anything in `client/js` or `client/views`
- `yarn dev` can be used to start The Lounge and watch for any file changes in the client folder
