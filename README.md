## Boilerplate Drupal theme with a modern development workflow

### Quick start
* Run `yarn` from the theme directory to install dependencies
* Copy the `.env.example to` file to a `.env` file:
  * Edit `DEV_URL`. It should reflect your local development hostname
* `yarn start` — Compile assets when file changes are made, start Browsersync session
* `yarn build` — Compile and optimize the files in your src directory for production

If Git hooks are not working, a Git repo was not initialized upon installation of packages.    Run `yarn add -D husky` to re-install.  
Husky sets up Git hooks on installation, and therefore needs a Git repository to be initialized beforehand. 


### Features
* Sass
* TypeScript
* Hot Module Replacement
* Code splitting with dynamic imports
* TSLint - extends [tslint:recommended](https://github.com/palantir/tslint/blob/master/src/configs/recommended.ts) and [tslint-eslint-rules](https://www.npmjs.com/package/tslint-eslint-rules)
* Stylelint - extends [stylelint-config-airbnb](https://www.npmjs.com/package/stylelint-config-airbnb) 
* Globally inlined Critical CSS, and/or based on node type 
* [PostCSS](https://github.com/postcss/postcss) - Transforming styles with JS plugins
* [Husky](https://github.com/typicode/husky) - Git hooks made easy, e.g. linting staged files before commit
* [Parceljs](https://parceljs.org//) - Blazing fast, zero configuration web application bundler
* [Browsersync](http://www.browsersync.io/) - Synchronized browser testing
* [sanitize.css](https://github.com/csstools/sanitize.css) - A best-practices CSS foundation
* [Adapt FE tools](https://www.npmjs.com/package/@adaptagency/fe_tools) - Utility collection to make development more easy and effecient


### Requirements
Make sure all dependencies have been installed before moving on:


* [Drupal](https://www.drupal.org//) > 8.x
* [Node.js](http://nodejs.org/) >= 8.0.0
* [Yarn](https://yarnpkg.com/en/docs/install)
* [Link CSS](https://www.drupal.org/project/link_css) - Drupal module needs to be enabled in development for Hot Module Reloading


### Theme installation
To be written...


### Theme structure

```shell
├── README.md
├── boilerplate.info.yml
├── boilerplate.libraries.yml
├── config
│   └── bs-config.js
├── package.json
├── public
│   ├── favicons
│   ├── fonts
│   └── icons
├── src
│   ├── abstractions
│   ├── base
│   ├── components
│   ├── main.ts
│   ├── main.scss
│   ├── mixins
│   └── settings
├── templates
│   ├── block
│   ├── content
│   ├── layout
│   ├── paragraphs
│   └── partials
├── yarn-error.log
└── yarn.lock
```

Drupal Paragraph components should go into `src/components` directory: 
```shell
src
├── components
    ├── README.md
    ├── accordion
    │   ├── accordion.ts
    │   └── accordion.scss
    └── simple-product
        ├── simple-product.scss
        └── simpleProduct.ts
```

### Theme setup
To be written...

### Theme development

* Run `yarn` from the theme directory to install dependencies
* Copy the `.env.example to` file to a `.env` file:
  * `DEV_URL` should reflect your local development hostname
  

### Build commands

* `yarn start` — Compile assets when file changes are made, start Browsersync session
* `yarn build` — Compile and optimize the files in your src directory for production
