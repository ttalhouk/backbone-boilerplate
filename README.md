![Boilerplate](https://github.com/tbranyen/backbone-boilerplate/raw/assets/header.png)

[![Build
Status](https://travis-ci.org/tbranyen/backbone-boilerplate.svg?branch=master)](https://travis-ci.org/backbone-boilerplate/backbone-boilerplate)
[![Coverage
Status](https://coveralls.io/repos/backbone-boilerplate/backbone-boilerplate/badge.png)](https://coveralls.io/r/backbone-boilerplate/backbone-boilerplate)
[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/backbone-boilerplate/backbone-boilerplate?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Backbone Boilerplate
====================

This boilerplate is the product of much research and frustration.  Existing
boilerplates freely modify Backbone core, lack a build process, and are very
prescriptive; Backbone Boilerplate changes that.

The Backbone Boilerplate is a way of organizing a web application with some
opinionated defaults, such as: [Backbone](http://backbonejs.org),
[jQuery](http://jquery.com), [Lodash](http://lodash.com),
[Grunt](http://gruntjs.com), [Babel](https://babeljs.io/),
[Combyne](https://github.com/tbranyen/combyne), Intern, PostCSS,
[Mocha](https://mochajs.org), and [PureCSS](http://purecss.io/) styles.

Organize your application with a logical file structure, develop your
Models/Collections/Views/Routers inside modules, and build knowing you have
efficient code that will not bottleneck your users.

Thanks to our
[Contributors](https://github.com/tbranyen/backbone-boilerplate/contributors)!
Special Thanks to: [cowboy](http://github.com/cowboy),
[iros](http://github.com/iros), [nimbupani](http://github.com/nimbupani),
[wookiehangover](http://github.com/wookiehangover), and
[jugglinmike](http://github.com/jugglinmike) for helping me create this
project.  Extra Special Thanks to: [Paul
Guinan](http://bigredhair.com/work/paul.html) for giving me usage rights to his
fantastic Boilerplate character.

## Documentation ##

[Backbone Boilerplate Wiki](https://github.com/tbranyen/backbone-boilerplate/wiki)

## Getting started ##

The easiest way to get started is to install Git and clone the repository:

``` bash
# Using Git, fetch only the latest commits.  You won't need the full history
# for your project.
git clone --depth 1 https://github.com/tbranyen/backbone-boilerplate

# Move the repository to your own project name.
mv backbone-boilerplate my-project
```

You will need to download and install [Node](http://nodejs.org/) to fetch the
dependencies and use the build tools.

## Updating dependencies ##

Third party packages may update independently from this main repo, so it's a
good idea to update after fetching.

``` bash
npm install
```

## Build process ##

The build process consists of numerous Grunt plugin tasks that work together
to optimize your application.

``` bash
# To run the build process, run the NPM start script. This will automatically
# run JSHint, the development Connect server, and watch your files for changes.
npm start

# Run a build and test the now optimized assets.
npm run test-prod
```

## Working with tests ##

Ceate an ES6 module in the `test/tests` directory and add an
import in the `test/runner.js` file. You'll see existing examples in there to
make it easy to follow.

Run the tests with:

``` bash
npm test
```

If you want to continuously test, run `npm start` and open the
`test/index.html` file in your browser. The tests will re-run whenever you
change source files.

By default, the test runner is BDD Mocha and uses Node's assert.

## License ##
Copyright © 2015 Tim Branyen (@tbranyen)  
Licensed under the MIT license.
