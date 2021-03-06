**EXPERIMENTAL: NOT INTENDED FOR PRODUCTION** There are definitely better solutions out there. Find one or build your own.

# Front-end Boilerplate

A full set of front-end development tools, based around NPM and Gulp.

[NPM](http://npmjs.org) is the standard package manager for Node. [Go here](http://nodejs.org) and click "Install" to get Node and NPM if you don't already have them. You won't need to use Node directly if you don't want to, so don't be concerned if you want to use something else as your back-end solution.

[Gulp](http://gulpjs.com) is a task management tool for building, testing and optimizing your web app projects. It takes care of all the boring-but-necessary tasks required to make high-quality web apps. Use ```npm install gulp -g``` to make Gulp available everywhere in your system.

## Features

Gulp gives you a bunch of great stuff without lifting a finger. It just happens every time you save your files.

- Sass compilation (to CSS)
- CSS autoprefixing
- CSS minification
- JSHint alerts
- JS uglification/minification/concatenation
- Image optimization
- Live Reload in the browser (no more refreshing!)
- Karma + Jasmine for JavaScript testing
- Built-in web server

## Coming Soon

- Cache-busting
- Gzipped assets
- UnCSS (removing unused rules on-the-fly)
- Browserify for client-side dependencies
- Hapi.js starter kit for Node dev

## Installation

- Clone this repo to your local system under your chosen project name
- Delete the ```.git``` directory
- ```git init; git add --all; git commit -m "Initial commit"``` to start a new, clean repo for your project
- ```npm init``` will prompt you for information about your project.
- ```npm install gulp gulp-ruby-sass gulp-autoprefixer gulp-minify-css gulp-jshint gulp-concat gulp-uglify gulp-imagemin gulp-notify gulp-rename gulp-livereload gulp-connect del karma karma-jasmine karma-chrome-launcher --save-dev``` will load all the components into a ```node_modules``` directory where NPM and Gulp can find them.
- ```gulp watch``` will start a server to serve your content on [http://localhost:8080](http://localhost:8080), live-reloading all your changes as you save your files. You'll need the [Chrome LiveReload extension](https://chrome.google.com/webstore/detail/livereload/jnihajbhpnppcggbcgedagnkighmdlei) for this to work. **NOTE** livereload only picks up edits to existing files: use ctrl-c to stop the watcher and restart to capture new html/js/img/styles.
- The code you edit is in the ```src``` directory structure:
  - ```html``` for HTML
  - ```scripts``` for Javascript
  - ```styles``` for Sass/CSS
  - ```images``` for images

  It will all be optimized and copied into the ```dist``` directory as you develop.
- Your Jasmine specs go in the ```test``` directory structure. An example has been provided. All specs will be rerun when your scripts or specs change.
- When you're ready to push your code to an actual web server, everything you need is in the ```dist``` directory: don't push the rest.
