# React Redux Webpack Boilerplate

## Features

This react boilerplate contains the following features:

- [Webpack 4](http://webpack.github.io) for bundling
- [Babel](http://babeljs.io) for transpiling ES6 and ES7
- [React](https://github.com/facebook/react)
- [React Router](https://github.com/rackt/react-router) with functional components and hooks
- [Redux](https://github.com/rackt/redux) for global state management with hooks
- [Redux Thunk Middleware](https://github.com/reduxjs/redux-thunk)
- [SCSS](https://sass-lang.com/), and CSS3 support
- [Jest/Enzyme](https://jestjs.io/) for adding unit tests & snapshot tests to the project
- [React-Helmet](https://github.com/nfl/react-helmet) to make your application SEO ready.

#### Development Features

- [Webpack Dev Server](https://webpack.js.org/configuration/dev-server/) A blazing fast local development server, with hot reloading
- React Hot Loader gives the ability to modify react components in real time, without reloading the page, and without losing component state when using webpack dev server
- [Redux Dev Tools](https://github.com/gaearon/redux-devtools) to easily navigate your redux store tree and see actions and their effects, live.
- [ESLint](http://eslint.org) to maintain a consistent code style throughout your application
- [Prettier](https://prettier.io/) to format code on save
- [Husky/Lint-Staged](https://github.com/typicode/husky) to make sure code is formatted correct pre commit, regardless or editor and environment

#### Production Optimizations

- Code Spltting bundle.js into two seperate files, one for vendor code, one for code written by us, for better caching.
- [UglifyJS Plugin](https://github.com/webpack-contrib/uglifyjs-webpack-plugin) for minifying JavaScript production files.
- [Optimize CSS Assets Plugin](https://github.com/NMFR/optimize-css-assets-webpack-plugin) for minifying CSS production file.
- [HTML Webpack Plugin](https://github.com/jantimon/html-webpack-plugin) for minimizing HTML production file.
- [Image Webpack Loader](https://github.com/jantimon/html-webpack-plugin) Reduces image sizes
  and many more including inlining small images into `bundle.js`
  and using css post loader to inject browser specfic styles into the final production stylesheet.css file

## Installation

```bash
npm install # install all the boilerplate dependencies
```

## Running Dev Server

```bash
npm run start # local webpack-dev-server with hot reloading
```

Start rapidly developing using the command above.

## Build Production

```bash
npm run build
```

This command will output your built web app in `dist/` folder. Thereafter you can copy and paste the contents of this folder to any static web host such as, [godaddy](https://godaddy.com), [hostpapa](https://hostpapa.com) into the public/root directory.
**It. Just. Works.**

If you would like to deploy to **modern web hosts**, it's even **easier**.

## Deployment on Surge.sh

**Pre-requiste:** Build Production first (to generate dist folder)

### Install Surge CLI Globally

```bash
npm install --g surge
```

### Deploy

In your project directory just run:

```bash
surge -p dist
```

After which you will be shown your project & domain name.
Hit `Enter` and it will build and deploy in a jiffy.

## Deployment on Heroku

TODO

## Deployment on Netlify

TODO

### Using Redux DevTools

[Redux Devtools](https://github.com/gaearon/redux-devtools) are enabled by default in development.

If you have the [Redux DevTools chrome extension](https://chrome.google.com/webstore/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd) installed it will automatically detect and you can start using it straight away.

<!-- DevTools are not enabled during production. -->

### Using The `public/` Folder

The `public/` folder located at the root of this boilerplate is where you can place, favicons, htacess, redirect files etc, that will automatically get added to the `dist/` when you build your project for production.

## Demo

A demonstration of this app can be seen [running on surge](http://boilerplate-redux.surge.sh)

<!-- , which is a deployment of the [netlify branch](https://github.com/erikras/react-redux-universal-hot-example/tree/heroku). -->

<!-- #### Images

Now it's possible to render the image both on client and server. Please refer to issue [#39](https://github.com/erikras/react-redux-universal-hot-example/issues/39) for more detail discussion, the usage would be like below (super easy):

```javascript
let logoImage = require('./logo.png');
``` -->

---

Thanks for checking this out.

– Kaiz Hudda, [@kaizhudda](https://twitter.com/kaizhudda)
