# myh.se
### A redesign of myh.se - the cooler version
This is a static website for myh.se which includes html and css files only.
Since we are using scss for this project, you should pre-install sass to your local machine.

## Install SASS

### Install anywhere (standalone)

You can install Sass on Windows, Mac, or Linux by downloading the package for your operating system from [GitHub](https://github.com/sass/dart-sass/releases/tag/1.26.11) and adding it to your [PATH](https://katiek2.github.io/path-doc/). 
### Install Anywhere (npm)
If you use Node.js, you can also install Sass using [npm](https://www.npmjs.com/) by running
```bash
npm install -g sass
```
### Install on Mac OS X or Linux (Homebrew)
If you use the [Homebrew package manager](https://brew.sh/) for Mac OS X or Linux, you can install Dart Sass by running
```bash
brew install sass/sass/sass
```

## How to compile scss files to css
The style.scss file includes all our style sheets. If you do not need to see your live changes in scss files, simply go to the ```styles ``` directory, run:
```bash
sass --watch style.scss:style.css
```
In this way, you might need to run this command above every time when you want to see the updates in your css changes. This might be annoying for many of you. Instead, go to the ```resources``` directory which locates in the root folder, run:
```bash
sass --watch styles/:styles/
```
Now you should be able to see your live changes in all static web pages if you have any updates in the related css files. 

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
