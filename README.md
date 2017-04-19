# npmdoc-react-autosuggest

#### api documentation for  [react-autosuggest (v9.0.0)](https://github.com/moroshko/react-autosuggest#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-autosuggest.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-autosuggest) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-autosuggest.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-autosuggest)

#### WAI-ARIA compliant React autosuggest component

[![NPM](https://nodei.co/npm/react-autosuggest.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-autosuggest)

- [https://npmdoc.github.io/node-npmdoc-react-autosuggest/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-autosuggest/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-autosuggest/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-autosuggest/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-autosuggest/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-autosuggest/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Misha Moroshko"
    },
    "bugs": {
        "url": "https://github.com/moroshko/react-autosuggest/issues"
    },
    "dependencies": {
        "react-autowhatever": "^9.1.0",
        "shallow-equal": "^1.0.0"
    },
    "description": "WAI-ARIA compliant React autosuggest component",
    "devDependencies": {
        "autoprefixer": "^6.7.5",
        "autosuggest-highlight": "^3.1.0",
        "babel-cli": "^6.23.0",
        "babel-core": "^6.23.1",
        "babel-eslint": "^7.1.1",
        "babel-loader": "^6.3.2",
        "babel-plugin-react-transform": "^2.0.2",
        "babel-plugin-transform-react-remove-prop-types": "^0.3.2",
        "babel-preset-es2015": "^6.22.0",
        "babel-preset-react": "^6.23.0",
        "babel-preset-stage-0": "^6.22.0",
        "babel-register": "^6.23.0",
        "chai": "^3.5.0",
        "cross-env": "^3.1.4",
        "css-loader": "^0.26.2",
        "es6-promise": "^4.0.5",
        "eslint": "^3.16.1",
        "eslint-plugin-react": "6.10.0",
        "extract-text-webpack-plugin": "^1.0.1",
        "file-loader": "^0.10.1",
        "ismobilejs": "^0.4.0",
        "isomorphic-fetch": "^2.2.1",
        "jsdom": "^9.11.0",
        "less": "^2.7.2",
        "less-loader": "^2.2.3",
        "mocha": "^3.2.0",
        "nyc": "^10.1.2",
        "openurl": "^1.1.1",
        "postcss-loader": "^1.3.2",
        "react": "^16.0.0-alpha.2",
        "react-addons-test-utils": "^16.0.0-alpha.2",
        "react-dom": "^16.0.0-alpha.2",
        "react-modal": "^1.6.5",
        "react-transform-hmr": "^1.0.4",
        "sinon": "^1.17.7",
        "sinon-chai": "^2.8.0",
        "style-loader": "^0.13.2",
        "svgo": "^0.7.2",
        "svgo-loader": "^1.1.2",
        "url-loader": "^0.5.8",
        "webpack": "^1.14.0",
        "webpack-dev-server": "^1.16.2"
    },
    "directories": {},
    "dist": {
        "shasum": "976b02e20d05615d05c328c8f1384daf98587821",
        "tarball": "https://registry.npmjs.org/react-autosuggest/-/react-autosuggest-9.0.0.tgz"
    },
    "files": [
        "dist"
    ],
    "gitHead": "f7fd6743a0299a0d4c3680e85f07831ebc57f33e",
    "homepage": "https://github.com/moroshko/react-autosuggest#readme",
    "keywords": [
        "autosuggest",
        "autocomplete",
        "auto-suggest",
        "auto-complete",
        "auto suggest",
        "auto complete",
        "react autosuggest",
        "react autocomplete",
        "react auto-suggest",
        "react auto-complete",
        "react auto suggest",
        "react auto complete",
        "react-autosuggest",
        "react-autocomplete",
        "react-auto-suggest",
        "react-auto-complete",
        "react-component"
    ],
    "license": "MIT",
    "main": "dist/index.js",
    "maintainers": [
        {
            "name": "moroshko"
        }
    ],
    "name": "react-autosuggest",
    "nyc": {
        "statements": 95,
        "branches": 91,
        "functions": 100,
        "lines": 95,
        "include": [
            "src/*.js"
        ],
        "exclude": [
            "test/**/*.js"
        ],
        "reporter": [
            "lcov",
            "text-summary"
        ],
        "require": [
            "babel-register",
            "./test/setup.js"
        ],
        "check-coverage": true
    },
    "optionalDependencies": {},
    "peerDependencies": {
        "react": ">=0.14.7 || >=16.0.0-alpha.2"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/moroshko/react-autosuggest.git"
    },
    "scripts": {
        "build": "npm run dist && npm run standalone",
        "copy-static-files": "cp demo/src/index.html demo/src/components/App/components/Examples/components/Basic/autosuggest.css demo/dist/",
        "demo-dist": "rm -rf demo/dist && mkdir demo/dist && npm run copy-static-files && cross-env BABEL_ENV=production webpack --config webpack.gh-pages.config.js",
        "dist": "rm -rf dist && mkdir dist && babel src -d dist",
        "gh-pages-build": "npm run prebuild && npm run demo-dist",
        "lint": "eslint src test demo/src demo/standalone/app.js server.js webpack.*.js",
        "postversion": "git push && git push --tags",
        "prebuild": "npm run lint && npm test",
        "prepublish": "npm run dist && npm run standalone",
        "standalone": "cross-env BABEL_ENV=production webpack --config webpack.standalone.config.js && webpack --config webpack.standalone-demo.config.js",
        "start": "mkdir -p demo/dist && npm run copy-static-files && node server",
        "test": "nyc mocha \"test/**/*.test.js\""
    },
    "version": "9.0.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
