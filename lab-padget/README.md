# Lab 23: Testing Angular Controllers

## Description
For this lab wrote a series of tests for our previous cow say app.

* [Cowsay](http://www.cowsays.com)

For more information see:
* [Class 23](https://github.com/codefellows/seattle-javascript-401d15/tree/master/class-23-testing-controllers)
* [Lab 23](https://github.com/codefellows-seattle-javascript-401d15/23-testing-controllers)
* [Class 22](https://github.com/codefellows/seattle-javascript-401d15/tree/master/class-22-angular-controllers)
* [Lab 22](https://github.com/codefellows-seattle-javascript-401d15/22-angular-controllers)

## Version
* 0.1.0

## Installation
Please visit the following pages for how to install your project locally.

* [Cloning A Repository](https://help.github.com/articles/cloning-a-repository/)
* [Fork A Repo](https://help.github.com/articles/fork-a-repo/)
* [Forking](https://guides.github.com/activities/forking/)

### Node
You need to have node.js installed.
* [Download Node](https://nodejs.org/en/)

### NPM Packages
* [NPM Docs](https://docs.npmjs.com)
* [NPM package.json](https://docs.npmjs.com/files/package.json)

### JSON Configuration
Initializing package.json
```
npm init

npm install -S angular babel-core babel-loader babel-preset-es2015 css-loader extract-text-webpack-plugin html-webpack-plugin node-sass sass-loader webpack style-loader

npm i -D angular-mocks jasmine jasmine-core karma karma-chrome-launcher karma-jasmine karma-webpack webpack-dev-server

npm install karma-mocha-reporter --save-dev

karma -init
```

Add the following to package.json:
```
"scripts": {
  "test": "karma start",
  "build": "webpack",
  "watch": "webpack-dev-server --inline --hot"
}

or

"scripts": {
  "test-watch": "karma start",
  "build": "webpack",
  "watch": "webpack-dev-server --inline --hot",
  "test": "karma start --single-run"
}
```

### Dependencies
The result of installation above.

```
"dependencies": {
  "angular": "^1.6.4",
  "babel-core": "^6.24.1",
  "babel-loader": "^7.0.0",
  "babel-preset-es2015": "^6.24.1",
  "css-loader": "^0.28.2",
  "extract-text-webpack-plugin": "^2.1.0",
  "html-webpack-plugin": "^2.28.0",
  "node-sass": "^4.5.3",
  "sass-loader": "^6.0.5",
  "style-loader": "^0.18.1",
  "webpack": "^2.6.1"
},
"devDependencies": {
  "angular-mocks": "^1.6.4",
  "jasmine": "^2.6.0",
  "jasmine-core": "^2.6.2",
  "karma": "^1.7.0",
  "karma-chrome-launcher": "^2.1.1",
  "karma-jasmine": "^1.1.0",
  "karma-webpack": "^2.0.3",
  "webpack-dev-server": "^2.4.5"
}
```

## Application
In Terminal run `webpack`
In Terminal run `npm run watch`

In your browser visit `http://localhost:8080/`

To change the cowsay ASCII art update index.js using the following resource:
https://helloacm.com/cowsay/

Add `$log.log(cowsay);` to index.js in the `CowsayController` function.
Open your console in the web browser and explore cowsay.

## Test Setup
```
karma init karma.conf.js

Which testing framework do you want to use ?
> jasmine

Do you want to use Require.js ?
> no

Do you want to capture any browsers automatically ?
> Chrome

What is the location of your source and test files ?
> test/**/*-test.js

Should any of the files included by the previous patterns be excluded ?
> no

Do you want Karma to watch all the files and run the tests on change ?
> no
```

## Running Tests
In [Bash](https://en.wikipedia.org/wiki/Bash_(Unix_shell)) (Terminal) enter the command:

karma start

## Resources
* [Testing Controllers](http://www.bradoncode.com/blog/2015/06/05/ngmock-fundamentals-testing-controllers/)
* [End to End Testing](https://docs.angularjs.org/guide/e2e-testing)
* [Testing with Protractor](http://www.ng-newsletter.com/posts/practical-protractor.html)
* [Protractor Tutorial](http://www.protractortest.org/#/tutorial)
* [Learn Angular](https://thinkster.io/a-better-way-to-learn-angularjs)
* [Guide to AngularJS](https://docs.angularjs.org/guide)
* [What is Webpack](https://webpack.github.io/docs/what-is-webpack.html)
* [Webpack Tutorial](https://webpack.github.io/docs/tutorials/getting-started/)

## License
This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/mmpadget/23-testing-controllers/blob/lab-23/lab-padget/LICENSE) file for details.

## Acknowledgments
* Code Fellows
* Scott Schmidt, Instructor
* Cayla Zabel, Teaching Assistant
* Devon Hackley, Teaching Assistant
* Thomas Martinez, Teaching Assistant
* JR Iriarte, Teaching Assistant
