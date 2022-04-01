## Hello everyone this is my fist **SASS/SCSS** project!!

Take a look at my website:
[Demo](https://)

> #### It was a fascinating experience to start using (SASS/SCSS) to write style the website and to use Gulp to compile this code of course with much more functions and features that I used gulp to implement.

.
.

## Well, now I wanna take you through my **(SCSS)** Code step by step!

_Are you excited let's start!!!_

.
.

### Notes - About the folders and files:

- _app_ directory => you can set your JS Folder, (SCSS/SASS) Folder, Images, and other components that are related to your website.

- _dist_ directory => you will find your complied CSS code that was compiled by gulp so set in it a CSS Folder <3.

- _node_modules_ => this folder will be created when you run it in your **terminal/cmd**:

  - npm install gulp so if you want to take a look at it just do it!!

- _gulpfile.js_ => Here is where the magic begins!! in this gulpfile.js you will write javascript code to compile your SCSS file and if you want to add another function, for instance, you can write a function for browsersync and so on.

- _index.html_ => your website structure.

- _package-lock.json_ is automatically generated for any operations where npm modifies either the node_modules tree or package. json [https://docs.npmjs.com].

- _package.json_ => created when you run in your terminal/cmd:
  npm init -y (and -y flag to say yes on all package.json questions)
  and its job is to hold metadata relevant to the project and it is used for managing the project's dependencies, scripts, version, and a whole lot more.

..

..

### How can I start my project?

- Firstly create a new folder NOTE: (if you are using the terminal/cmd watch the box below!).

- Open it using your code editor.

- Open the terminal and run:
  npm init -y (to start the packge.josn file)
  npm install @babel/core @babel/preset-env postcss autoprefixer browser-sync cssnano dart-sass sass gulp gulp-babel gulp-postcss gulp-sass gulp-terser

  > here you go now you have your project started!!

- You should see now package.json file, package-lock.json file, and, node_modules folder.

- Create your app folder dist one and the files => gulpfile.js, index.html!

### Are comfortable with CMD/Terminal? follow these steps to set your project!

    - cd desktop/documents (open any directory you want)
    - mkdir project (after mkdir command write the projectName)
    - cd project (open the projectName)
    - npm init -y (the -y flag to sey yes to every question)
    - npm install @babel/core @babel/preset-env postcss autoprefixer browser-sync cssnano dart-sass sass gulp gulp-babel gulp-postcss gulp-sass gulp-terser

**Every thing is set to up? KEEP MOVING!**

#### SCSS explination for the code:

##### We start our scss file with this code

`$colors:( primary: #005DFF, primary-light: lighten(#005DFF, 40%), primary-dark: darken(#005DFF, 40%), accent: #FFF6BB, ); `

     This code looks like objects/dictionaries to save the variables it is not necessary to be a colors it might be a font-sizes or paddings values and so on. fine, now how can I use it? well now you need to meet our friend the:

> **map-get()** function, this function take tow pramemtars the first: the name of the map (object / dectionary) and the second a key form it. Ohhh it look like the Object.keys() & Object.values() in JS isn't it??

> The second two lines

`$padding: 15px; $desktop: 840px;`

> This is the way that you can create a variable in (SASS/SCSS)!

> The @mixin at-rule defined by tow ways:

- First: @mixin <name> { @content }
- Second: @mixin name(<arguments...>) { @content }.

Notes on @mixin:

- A mixin’s name can be any Sass identifier.
- Mixins are included into the current context using the @include at-rule, which is written @include <name> or @include <name>(<arguments...>)

`@function color($clr){ @return map-get($colors, $clr); } `

This code shows you how you can make a function within SASS/SCSS file this function keeps you away from writing map-get($map-name, value) each time you wanna use it...

_And the rest is just a nested regular style!!_

#### Thank you for reading this READme file.

It was me **Wajd Wael**, see you with the next repo and a next readme file.

**_Best Wishes..._**
