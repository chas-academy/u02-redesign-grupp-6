# A redesign of myh.se - the cooler version :sunglasses:
This is a static website for myh.se which includes html and scss files only.
Since we are using scss for this project, you should pre-install sass to your local machine.

## How we structure our files
All the html files have one and the same one stylesheet which is ```style.css```. Style.css includes all the css for our static website by ```@import``` all scss files.
So this will create one issue, when you open any page the ```style.css``` will always try to load all the css into one big css file and serves it. For instance, if you open the homepage the ```index.html``` will look for ```style.css``` which contains all the css including ```index.css``` and many other css files, such as ```footer.css```, ```navbar.css```, and etc. When you are giving class names to the html files, please do not make a too generic class name, such as ```body```. Furthermore, avoid styling the semantic elemnets directly, such as ```h1 {font-size=16px}``` because it might interfere with other html files where they also have ```h1```.

## Before you jump into the project, install SASS! :stuck_out_tongue_winking_eye:

### How to install SASS

### Install anywhere (standalone)

You can install Sass on Windows, Mac, or Linux by downloading the package for your operating system from [GitHub](https://github.com/sass/dart-sass/releases/tag/1.26.11) and adding it to your [PATH](https://katiek2.github.io/path-doc/). 
### Install anywhere (npm)
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
In this way, you might need to run this command above every time when you want to see the updates in your css changes. This might be annoying for many of you. Instead, go to the ```resources``` directory which locates in the root folder.
```bash 
cd resources/
``` 

```bash
sass --watch styles/:styles/
```
Now you should be able to see your live changes in all static web pages if you have any updates in the related css files. 

### If you use [Live Sass Compiler](https://marketplace.visualstudio.com/items?itemName=ritwickdey.live-sass) to compile scss to css in [Visual Studio Code](https://code.visualstudio.com/):point_left:
Unfortunately, our team members have encountered problems using this plugin. It is not compiling the style.scss once there is changes in other scss files. We highly recommend you to run the ```sass --watch styles/:styles/``` on your terminal instead. We appreciate if you find a solution with the plugin in Vscode and let us know.

## Contributing :heart:
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. 

### Join our developer team :sparkles:
As of now, we have six developers working in the frontend team, and of course we would like to expand the team! We are using [trello](https://trello.com/en) to collaborate and [slack](https://slack.com/intl/en-se/) to communicate.If you are interested in joining us, please talk to our brilliant scrum master, [Otto](https://github.com/ottoreimers)! :v:
