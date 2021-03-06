# Reveal.js Boilerplate

This is a boilerplate to use [Reveal.JS](http://lab.hakim.se/reveal-js/) easily with [Gulp](http://gulpjs.com/), [Jade](http://jade-lang.com/) and [Stylus](http://learnboost.github.io/stylus/).

To know more about Reveal.js and how to use, [read the docs here](https://github.com/hakimel/reveal.js).


## Getting Started

### Installation

First of all, install the dependencies to run this boilerplate.

- [NodeJS](http://nodejs.org/)
- [GulpJS](http://gulpjs.com/)

```sh
# Clone this repository
$ git clone git://github.com/willianjusten/reveal-boilerplate.git new_project
$ cd new_project

# install dependencies
$ npm install
# run tasks and serve
$ gulp
```

With the commands above, you have everything to start.

```sh
new_project -
	/build -
		/css
			main.css
		/js
		    /vendor
			main.js
		index.html
	/src -
		/js
		/slides
		/styl
			/highlight-themes
			/reveal-themes
			/vendor
			main.styl
		/templates
			/inc
				head.jade
				scripts.jade
	.gitignore	
	gulpfile.js
	package.json
	Readme.md
```

### How to Use

- Write your slides in `src/slides` folder in separated files using the [jade syntax](http://jade-lang.com/) and add them on `templates/index.jade`.

- If you want to add another scripts and css use the `templates/inc/` folder and call them in the  `templates/index.jade`.

### Tasks

- `gulp`: Initialize watch for changes and a server(localhost:3000)
- `gulp js`: execute js files
- `gulp notes`: copy speaker notes
- `gulp stylus`: compile stylus files
- `gulp imagemin`:compress image files
- `gulp watch`: call for watch files
- `gulp jade`: compile jade files
- `gulp deploy-pages`: deploy compiled files at `build` to `github` on branch `gh-pages`.
- `gulp deploy-src`: deploy compiled files at `build` to `github pages` on branch `master`.