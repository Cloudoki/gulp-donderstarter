# Gulp-donderstarter
Base for static front-end development using gulp, sass and bower

## Features
- Gulp;
- Bower to manage dependencies;
- CSS pre-compile through SASS;
- JShint;
- SASS and JS minification and concatenation;

## Requirements
- [nodejs](https://nodejs.org/)
- [npm](https://www.npmjs.com/)

## Install
Install the dependencies with `npm install` or `sudo npm install`. Then just run `gulp`.

## Images
If you want to add image files, creating an `/images` folder directly on the `/src` will include them in the gulp build task.

## Adding packages
The donderstarters are setup so you can easily add external packages to your project, while making it easier to manage dependencies. Doing
`bower install <package-name>` will add the package to the src/vendor folder. You can browse for available bower packages through [bower search page](http://bower.io/search/), and general documentation on bower in [bower.io](http://bower.io/).

After adding the package, you need to include it into the build process (gulpfile.js:38) and into your index.html file (index.html:19). Both have documented examples in the files themselves. 

## Gulp tasks
- **gulp** will build the files inside the /dist folder and perform a watch. You are ready to start developing
- **gulp build** will build the files inside the /dist folder. No watcher.
- **gulp clean** will clean the dist folder
- **gulp release** will do the same build but with a js uglify in the end