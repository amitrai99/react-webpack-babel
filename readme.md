# Setting Up a React.js Environment Using Npm, Babel 6 and Webpack

init NPM

```bash
npm init
```

## Installing and Configuring Webpack
```bash
npm i webpack -S
touch webpack.config.js
```

Run webpack in dev

```bash
./node_modules/.bin/webpack -d
```

## Setting Up Babel-Loader

The babel-preset-es2015 and babel-preset-react are plugins being used by the babel-loader to translate ES6 and JSX syntax respectively.

```bash
npm i babel-loader babel-preset-es2015 babel-preset-react -S
touch .babelrc
```

##React

```bash
npm i react react-dom -S
```

## Making Webpack Watch Changes

```
./node_modules/.bin/webpack -d --watch
```

## Using npm as a tool runner

Update `packages.json`

```js
"scripts": {
    "dev": "webpack -d --watch",
    "build" : "webpack -p"
  }
```


```bash
# the command npm run build runs Webpack in production mode
npm run build
# command npm run dev runs the Webpack in the watch mode
npm run dev
```



Original article:

https://www.codementor.io/reactjs/tutorial/beginner-guide-setup-reactjs-environment-npm-babel-6-webpack
