# api documentation for  [react-autosuggest (v9.0.0)](https://github.com/moroshko/react-autosuggest#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-autosuggest.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-autosuggest) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-autosuggest.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-autosuggest)
#### WAI-ARIA compliant React autosuggest component

[![NPM](https://nodei.co/npm/react-autosuggest.png?downloads=true)](https://www.npmjs.com/package/react-autosuggest)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-autosuggest/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-react-autosuggest_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-autosuggest/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-autosuggest/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-autosuggest/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Misha Moroshko",
        "email": "michael.moroshko@gmail.com"
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
            "name": "moroshko",
            "email": "michael.moroshko@gmail.com"
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
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module react-autosuggest](#apidoc.module.react-autosuggest)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.</span>propTypes.alwaysRenderSuggestions ()](#apidoc.element.react-autosuggest.propTypes.alwaysRenderSuggestions)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.</span>propTypes.id ()](#apidoc.element.react-autosuggest.propTypes.id)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.</span>propTypes.onSuggestionSelected ()](#apidoc.element.react-autosuggest.propTypes.onSuggestionSelected)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.</span>propTypes.theme ()](#apidoc.element.react-autosuggest.propTypes.theme)
1.  object <span class="apidocSignatureSpan">react-autosuggest.</span>defaultProps
1.  object <span class="apidocSignatureSpan">react-autosuggest.</span>propTypes

#### [module react-autosuggest.defaultProps](#apidoc.module.react-autosuggest.defaultProps)
1.  boolean <span class="apidocSignatureSpan">react-autosuggest.defaultProps.</span>alwaysRenderSuggestions
1.  boolean <span class="apidocSignatureSpan">react-autosuggest.defaultProps.</span>focusInputOnSuggestionClick
1.  boolean <span class="apidocSignatureSpan">react-autosuggest.defaultProps.</span>highlightFirstSuggestion
1.  boolean <span class="apidocSignatureSpan">react-autosuggest.defaultProps.</span>multiSection
1.  [function <span class="apidocSignatureSpan">react-autosuggest.defaultProps.</span>renderSuggestionsContainer (_ref)](#apidoc.element.react-autosuggest.defaultProps.renderSuggestionsContainer)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.defaultProps.</span>shouldRenderSuggestions (value)](#apidoc.element.react-autosuggest.defaultProps.shouldRenderSuggestions)
1.  object <span class="apidocSignatureSpan">react-autosuggest.defaultProps.</span>theme
1.  string <span class="apidocSignatureSpan">react-autosuggest.defaultProps.</span>id

#### [module react-autosuggest.propTypes](#apidoc.module.react-autosuggest.propTypes)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>alwaysRenderSuggestions ()](#apidoc.element.react-autosuggest.propTypes.alwaysRenderSuggestions)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>focusInputOnSuggestionClick ()](#apidoc.element.react-autosuggest.propTypes.focusInputOnSuggestionClick)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>getSectionSuggestions (props, propName)](#apidoc.element.react-autosuggest.propTypes.getSectionSuggestions)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>getSuggestionValue ()](#apidoc.element.react-autosuggest.propTypes.getSuggestionValue)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>highlightFirstSuggestion ()](#apidoc.element.react-autosuggest.propTypes.highlightFirstSuggestion)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>id ()](#apidoc.element.react-autosuggest.propTypes.id)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>inputProps (props, propName)](#apidoc.element.react-autosuggest.propTypes.inputProps)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>multiSection ()](#apidoc.element.react-autosuggest.propTypes.multiSection)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>onSuggestionSelected ()](#apidoc.element.react-autosuggest.propTypes.onSuggestionSelected)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>onSuggestionsClearRequested (props, propName)](#apidoc.element.react-autosuggest.propTypes.onSuggestionsClearRequested)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>onSuggestionsFetchRequested (props, propName)](#apidoc.element.react-autosuggest.propTypes.onSuggestionsFetchRequested)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>renderInputComponent ()](#apidoc.element.react-autosuggest.propTypes.renderInputComponent)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>renderSectionTitle (props, propName)](#apidoc.element.react-autosuggest.propTypes.renderSectionTitle)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>renderSuggestion ()](#apidoc.element.react-autosuggest.propTypes.renderSuggestion)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>renderSuggestionsContainer ()](#apidoc.element.react-autosuggest.propTypes.renderSuggestionsContainer)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>shouldRenderSuggestions ()](#apidoc.element.react-autosuggest.propTypes.shouldRenderSuggestions)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>suggestions ()](#apidoc.element.react-autosuggest.propTypes.suggestions)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>theme ()](#apidoc.element.react-autosuggest.propTypes.theme)

#### [module react-autosuggest.propTypes.alwaysRenderSuggestions](#apidoc.module.react-autosuggest.propTypes.alwaysRenderSuggestions)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>alwaysRenderSuggestions ()](#apidoc.element.react-autosuggest.propTypes.alwaysRenderSuggestions.alwaysRenderSuggestions)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.alwaysRenderSuggestions.</span>isRequired ()](#apidoc.element.react-autosuggest.propTypes.alwaysRenderSuggestions.isRequired)

#### [module react-autosuggest.propTypes.id](#apidoc.module.react-autosuggest.propTypes.id)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>id ()](#apidoc.element.react-autosuggest.propTypes.id.id)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.id.</span>isRequired ()](#apidoc.element.react-autosuggest.propTypes.id.isRequired)

#### [module react-autosuggest.propTypes.onSuggestionSelected](#apidoc.module.react-autosuggest.propTypes.onSuggestionSelected)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>onSuggestionSelected ()](#apidoc.element.react-autosuggest.propTypes.onSuggestionSelected.onSuggestionSelected)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.onSuggestionSelected.</span>isRequired ()](#apidoc.element.react-autosuggest.propTypes.onSuggestionSelected.isRequired)

#### [module react-autosuggest.propTypes.theme](#apidoc.module.react-autosuggest.propTypes.theme)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>theme ()](#apidoc.element.react-autosuggest.propTypes.theme.theme)
1.  [function <span class="apidocSignatureSpan">react-autosuggest.propTypes.theme.</span>isRequired ()](#apidoc.element.react-autosuggest.propTypes.theme.isRequired)



# <a name="apidoc.module.react-autosuggest"></a>[module react-autosuggest](#apidoc.module.react-autosuggest)

#### <a name="apidoc.element.react-autosuggest.propTypes.alwaysRenderSuggestions"></a>[function <span class="apidocSignatureSpan">react-autosuggest.</span>propTypes.alwaysRenderSuggestions ()](#apidoc.element.react-autosuggest.propTypes.alwaysRenderSuggestions)
- description and source-code
```javascript
propTypes.alwaysRenderSuggestions = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.id"></a>[function <span class="apidocSignatureSpan">react-autosuggest.</span>propTypes.id ()](#apidoc.element.react-autosuggest.propTypes.id)
- description and source-code
```javascript
propTypes.id = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.onSuggestionSelected"></a>[function <span class="apidocSignatureSpan">react-autosuggest.</span>propTypes.onSuggestionSelected ()](#apidoc.element.react-autosuggest.propTypes.onSuggestionSelected)
- description and source-code
```javascript
propTypes.onSuggestionSelected = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.theme"></a>[function <span class="apidocSignatureSpan">react-autosuggest.</span>propTypes.theme ()](#apidoc.element.react-autosuggest.propTypes.theme)
- description and source-code
```javascript
propTypes.theme = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-autosuggest.defaultProps"></a>[module react-autosuggest.defaultProps](#apidoc.module.react-autosuggest.defaultProps)

#### <a name="apidoc.element.react-autosuggest.defaultProps.renderSuggestionsContainer"></a>[function <span class="apidocSignatureSpan">react-autosuggest.defaultProps.</span>renderSuggestionsContainer (_ref)](#apidoc.element.react-autosuggest.defaultProps.renderSuggestionsContainer)
- description and source-code
```javascript
function defaultRenderSuggestionsContainer(_ref) {
  var containerProps = _ref.containerProps,
      children = _ref.children;
  return _react2.default.createElement(
    'div',
    containerProps,
    children
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.defaultProps.shouldRenderSuggestions"></a>[function <span class="apidocSignatureSpan">react-autosuggest.defaultProps.</span>shouldRenderSuggestions (value)](#apidoc.element.react-autosuggest.defaultProps.shouldRenderSuggestions)
- description and source-code
```javascript
function defaultShouldRenderSuggestions(value) {
  return value.trim().length > 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-autosuggest.propTypes"></a>[module react-autosuggest.propTypes](#apidoc.module.react-autosuggest.propTypes)

#### <a name="apidoc.element.react-autosuggest.propTypes.alwaysRenderSuggestions"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>alwaysRenderSuggestions ()](#apidoc.element.react-autosuggest.propTypes.alwaysRenderSuggestions)
- description and source-code
```javascript
alwaysRenderSuggestions = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.focusInputOnSuggestionClick"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>focusInputOnSuggestionClick ()](#apidoc.element.react-autosuggest.propTypes.focusInputOnSuggestionClick)
- description and source-code
```javascript
focusInputOnSuggestionClick = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.getSectionSuggestions"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>getSectionSuggestions (props, propName)](#apidoc.element.react-autosuggest.propTypes.getSectionSuggestions)
- description and source-code
```javascript
function getSectionSuggestions(props, propName) {
  var getSectionSuggestions = props[propName];

  if (props.multiSection === true && typeof getSectionSuggestions !== 'function') {
    throw new Error('\'getSectionSuggestions\' must be implemented. See: https://github.com/moroshko/react-autosuggest#getSectionSuggestionsProp
');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.getSuggestionValue"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>getSuggestionValue ()](#apidoc.element.react-autosuggest.propTypes.getSuggestionValue)
- description and source-code
```javascript
getSuggestionValue = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.highlightFirstSuggestion"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>highlightFirstSuggestion ()](#apidoc.element.react-autosuggest.propTypes.highlightFirstSuggestion)
- description and source-code
```javascript
highlightFirstSuggestion = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.id"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>id ()](#apidoc.element.react-autosuggest.propTypes.id)
- description and source-code
```javascript
id = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.inputProps"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>inputProps (props, propName)](#apidoc.element.react-autosuggest.propTypes.inputProps)
- description and source-code
```javascript
function inputProps(props, propName) {
  var inputProps = props[propName];

  if (!inputProps.hasOwnProperty('value')) {
    throw new Error('\'inputProps\' must have \'value\'.');
  }

  if (!inputProps.hasOwnProperty('onChange')) {
    throw new Error('\'inputProps\' must have \'onChange\'.');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.multiSection"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>multiSection ()](#apidoc.element.react-autosuggest.propTypes.multiSection)
- description and source-code
```javascript
multiSection = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.onSuggestionSelected"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>onSuggestionSelected ()](#apidoc.element.react-autosuggest.propTypes.onSuggestionSelected)
- description and source-code
```javascript
onSuggestionSelected = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.onSuggestionsClearRequested"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>onSuggestionsClearRequested (props, propName)](#apidoc.element.react-autosuggest.propTypes.onSuggestionsClearRequested)
- description and source-code
```javascript
function onSuggestionsClearRequested(props, propName) {
  var onSuggestionsClearRequested = props[propName];

  if (props.alwaysRenderSuggestions === false && typeof onSuggestionsClearRequested !== 'function') {
    throw new Error('\'onSuggestionsClearRequested\' must be implemented. See: https://github.com/moroshko/react-autosuggest#onSuggestionsClearRequestedProp
');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.onSuggestionsFetchRequested"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>onSuggestionsFetchRequested (props, propName)](#apidoc.element.react-autosuggest.propTypes.onSuggestionsFetchRequested)
- description and source-code
```javascript
function onSuggestionsFetchRequested(props, propName) {
  var onSuggestionsFetchRequested = props[propName];

  if (typeof onSuggestionsFetchRequested !== 'function') {
    throw new Error('\'onSuggestionsFetchRequested\' must be implemented. See: https://github.com/moroshko/react-autosuggest#onSuggestionsFetchRequestedProp
');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.renderInputComponent"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>renderInputComponent ()](#apidoc.element.react-autosuggest.propTypes.renderInputComponent)
- description and source-code
```javascript
renderInputComponent = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.renderSectionTitle"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>renderSectionTitle (props, propName)](#apidoc.element.react-autosuggest.propTypes.renderSectionTitle)
- description and source-code
```javascript
function renderSectionTitle(props, propName) {
  var renderSectionTitle = props[propName];

  if (props.multiSection === true && typeof renderSectionTitle !== 'function') {
    throw new Error('\'renderSectionTitle\' must be implemented. See: https://github.com/moroshko/react-autosuggest#renderSectionTitleProp
');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.renderSuggestion"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>renderSuggestion ()](#apidoc.element.react-autosuggest.propTypes.renderSuggestion)
- description and source-code
```javascript
renderSuggestion = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.renderSuggestionsContainer"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>renderSuggestionsContainer ()](#apidoc.element.react-autosuggest.propTypes.renderSuggestionsContainer)
- description and source-code
```javascript
renderSuggestionsContainer = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.shouldRenderSuggestions"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>shouldRenderSuggestions ()](#apidoc.element.react-autosuggest.propTypes.shouldRenderSuggestions)
- description and source-code
```javascript
shouldRenderSuggestions = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.suggestions"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>suggestions ()](#apidoc.element.react-autosuggest.propTypes.suggestions)
- description and source-code
```javascript
suggestions = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.theme"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>theme ()](#apidoc.element.react-autosuggest.propTypes.theme)
- description and source-code
```javascript
theme = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-autosuggest.propTypes.alwaysRenderSuggestions"></a>[module react-autosuggest.propTypes.alwaysRenderSuggestions](#apidoc.module.react-autosuggest.propTypes.alwaysRenderSuggestions)

#### <a name="apidoc.element.react-autosuggest.propTypes.alwaysRenderSuggestions.alwaysRenderSuggestions"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>alwaysRenderSuggestions ()](#apidoc.element.react-autosuggest.propTypes.alwaysRenderSuggestions.alwaysRenderSuggestions)
- description and source-code
```javascript
alwaysRenderSuggestions = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.alwaysRenderSuggestions.isRequired"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.alwaysRenderSuggestions.</span>isRequired ()](#apidoc.element.react-autosuggest.propTypes.alwaysRenderSuggestions.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-autosuggest.propTypes.id"></a>[module react-autosuggest.propTypes.id](#apidoc.module.react-autosuggest.propTypes.id)

#### <a name="apidoc.element.react-autosuggest.propTypes.id.id"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>id ()](#apidoc.element.react-autosuggest.propTypes.id.id)
- description and source-code
```javascript
id = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.id.isRequired"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.id.</span>isRequired ()](#apidoc.element.react-autosuggest.propTypes.id.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-autosuggest.propTypes.onSuggestionSelected"></a>[module react-autosuggest.propTypes.onSuggestionSelected](#apidoc.module.react-autosuggest.propTypes.onSuggestionSelected)

#### <a name="apidoc.element.react-autosuggest.propTypes.onSuggestionSelected.onSuggestionSelected"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>onSuggestionSelected ()](#apidoc.element.react-autosuggest.propTypes.onSuggestionSelected.onSuggestionSelected)
- description and source-code
```javascript
onSuggestionSelected = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.onSuggestionSelected.isRequired"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.onSuggestionSelected.</span>isRequired ()](#apidoc.element.react-autosuggest.propTypes.onSuggestionSelected.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-autosuggest.propTypes.theme"></a>[module react-autosuggest.propTypes.theme](#apidoc.module.react-autosuggest.propTypes.theme)

#### <a name="apidoc.element.react-autosuggest.propTypes.theme.theme"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.</span>theme ()](#apidoc.element.react-autosuggest.propTypes.theme.theme)
- description and source-code
```javascript
theme = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-autosuggest.propTypes.theme.isRequired"></a>[function <span class="apidocSignatureSpan">react-autosuggest.propTypes.theme.</span>isRequired ()](#apidoc.element.react-autosuggest.propTypes.theme.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
