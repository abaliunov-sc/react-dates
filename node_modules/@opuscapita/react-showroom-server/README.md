# Node - Showroom Server

## Synopsis

Server side for [opuscapita-showroom-client](https://github.com/OpusCapitaBES/js-react-showroom-client).

## Motivation to develop

* Easily browsing react components with examples to pick the most appropriate component for your current task
* Provide an **always actual documentation**

## Usage

* Clone repository

  ```shell
  git clone https://github.com/OpusCapitaBES/js-node-showroom-server
  ```

* Install dependencies

  ```shell
  npm install
  ```

* Host and port configuration [here](./serverConfig.js)

* Run this goal (see configuration below)

  ```shell
  npm run init-packages
  ```

### What this goal do:

  * Remove **packages installation root** directory named specified [here](./src/tools/npm-installer/config.js)

  * Install **packages list** specified [here](./src/tools/npm-installer/config.js)

  * Scan npm packages directories to find components. Only documented components will be added. Config [here](./src/tools/npm-scanner/config.js)

  * Make bundles using [webpack configuration](./src/tools/npm-bundler/webpack.config.js). **Maybe you should not change it**

  * Components **must** be available as fields of [npm package main file](https://docs.npmjs.com/files/package.json#main)

## Roadmap

* Improve init-packages process
* Make Docker container for easy deploy and update

## Contributors

* Alexey Sergeev - [alexey.sergeev@jcatalog.com](alexey.sergeev@jcatalog.com)
* Kirill Volkovich - [kirill.volkovich@jcatalog.com](kirill.volkovich@jcatalog.com)

## License

OpusCapita 2016
