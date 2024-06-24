# odin-21-express-local-library

A template for beginning an express application, which has been created by following the set-by-step guide below, which allows it to be re-created if necessary.

## Using the template

Clone this repository.

## Install the express-generator

Install the application generator globally if it hasn't been already:

```bash
$ npm install -g express-generator
$ express
```

## Create the express project

Create the project in the current directory, and install dependencies.
CHECK THIS WORKS FOR CURRENT DIRECTORY - NOT TESTED
This sets the view engine to Pug

```bash
 express --view=pug
 npm install
```

Start the project, enabling console logging

```bash
SET DEBUG=express-locallibrary-tutorial:* & npm start
```

##Install nodemon to enable live updates of the server

(Could instead install this globally.)
Note, a page refresh is still necessary to see the changes.

```bash
npm install --save-dev nodemon
```

## Add npm scripts for ease

```js
  "scripts": {
    "devstart": "nodemon ./bin/www",
    "serverstart": "DEBUG=nameoftheapp:* npm run devstart"
  },
```

## Bring the dependency versions up to date

**package.json**

```js
  "dependencies": {
    "cookie-parser": "^1.4.6",
    "debug": "^4.3.5",
    "express": "^4.19.2",
    "http-errors": "~2.0.0",
    "morgan": "^1.10.0",
    "pug": "3.0.3"
  },
```

```pug
npm install
```

## Install Mongoose

Installing mongoose installs all its dependencies and the MongoDB database driver, but not MongoDB itself.

```bash
npm install mongoose
```
