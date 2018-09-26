# concomitant

Concomitant, first Balticum talents serious project. Modified to reflect my skills. 
This project was meant to create almost identical design copy.

Live version currently unavailable. Live version will be available as soon as project is finished

## Total time spent on this project.
```
35 minutes 09-25-2018 (branch slideshow)
1h 22minutes 09-25-2018 (branch table-row)
52min 09-25-2018 (branch project-title-table)
1h:18min 09-25-2018 (branch contact-info)
43min 09-26-2018 (branch bug-fix)
```
## Bugs or not implemented features.
```
Major:
1.Need to create working slideshow with javascript (https://www.w3schools.com/howto/tryit.asp?filename=tryhow_js_slideshow)
Use real pictures
2.Contact info read more link to close to 4 block.
Medium:
3.Change writing color to white. in send email section
4.Create lazyloading
Minor:
1.When hovering over twitter icon size sligtly increase. 
2. Title design need borders
4. Search button left border shorter then it should be.
4. Table need to be responsive. (Design too small not a real website)
```
Bug Fixed
```
Medium
1.Need to fix slideshow controls. Put them slightly higher. 09/26/2018
2.Fix slideshow background. Darker background around the picture. 09/26/2018
Minor:
1.Search bar dosen't seem quite right. 09/26/2018
2.Title shorter then in design. 09/26/2018
3. Add space in project title name. 09/26/2018

```
## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

```
Node.js from Node.js website. For npm packages.
```

### Installing

A step by step series of examples that tell you how to get a development env running

Open command prompt in project root folder and type:

```
npm install
```
To deploy server for editing with gulp enabled:
```
gulp watch
```
## Icons

IMPORTANT all svg files must be placed in app\assets\images\icons folder.
To combine all svg files into one write:

```
gulp icons
```

Combines icons files appear at:

```
app\assets\images\sprites\sprite-e79e95cc.svg
```
Please note there is also a backup png sprites to support older browsers.
To use your icon in the project:

add class into div from:
```
app\assets\styles\modules\_sprite.css
```
Example For a facebook icon.
```
 <div class = "icon icon--facebook"></div>
```
## Deployment

To deploy on live system you need to bundle all files together. You can do this in git bash writing:

```
gulp build
```
To preview your build project write in git bash

```
gulp previewdist
```
## Changing deployed folder name from docs to your choosing.

Sometimes you need to change your distribution folder name, to change it,
modify these lines name "docs" to name you want to have.

gulp\tasks\build.js
```
14 line (baseDir: "docs"),
20 line (return del('./docs')),
36 line (.pipe(gulp.dest("./docs"));)
48 line .pipe(gulp.dest('./docs/assets/images'));
61 line .pipe(gulp.dest("./docs"));
```

## Built With

* [BABEL](https://github.com/babel/babel) - For writing modern javascript.
* [WEBPACK](https://github.com/webpack/webpack) - For bundling javascript files.
* [JQUERY](https://github.com/jquery/jquery) - Javascript library.
* [POSTCSS](https://github.com/postcss/postcss) - For styling files.
* [GULP](https://github.com/gulpjs/gulp) - For automating browser.

## Authors

* **Arnas Dickus**

## Acknowledgments

* Thanks to Balticum Talents for providing me a design
