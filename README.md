Ready? Set. Go!
---------------

This is a barebones package to get started with Gulp and managing any of your packages with Bower neatly put together by @MattLePhoto.

Enjoy, tweak, springboard, change the world. 


Install Packages with Bower
---------------
With Bower you can manage all your packages in one place and source control their versions. This step is optional. 

### Install Bower

Bower Site - http://bower.io/

#### 1. Install bower globally:

```sh
$ npm install -g bower
```

#### 2. Install bower dependencies in your project folder:

```sh
$ bower init
```

#### 3. Install any package you want:

```sh
$ bower install bootstrap-sass-official --save  
$ bower install fontawesome --save
```


Setting up Gulp
---------------
Gulp is used as the task runner that preprocesses all of your stylesheets, javascript, etc. Follow these command lines to get up and running with Gulp. 

### Install Gulp

Gulp Site - http://gulpjs.com/

#### 1. Install gulp globally:

```sh
$ npm install --global gulp
```

#### 2. Install gulp dependencies in your project:

```sh
$ npm install --save-dev gulp
```

#### 3. Download and install required node packages:

```sh
$ npm install gulp-bower gulp-sass gulp-autoprefixer gulp-minify-css gulp-jshint gulp-concat gulp-uglify gulp-imagemin gulp-notify gulp-rename gulp-livereload gulp-cache del --save-dev
```

#### 4. Run gulp:

```sh
$ gulp
```

Here are a few notable tasks you can run form this setup. To view the entire list, please view the package.json file. 

Tasks with Gulp
===

To gain the full benefits of Flint's Gulp setup, please see the following example commands: 

**Compiling and optimizing tasks:**

| Command   |      Task(s)      |
|----------|:-------------:|
| `styles` | Compile all *.scss* files in src/sass directory |
| `scripts` |    Compile all vendor and plugin *.js* files   |
| `images` |    Optimize images within the src/images directory   |
| **`default`** |    Run `styles`, `scripts`, and `images` simultaneously   |

**Automated tasks:**

| Command   |      Task(s)      |
|----------|:-------------:|
| `watch` |  Run Watch for *.scss*, *.js*, and *.html* () |
| `sync` |    Run Browser-Sync    |
