# npmtest-react-timeago

#### basic test coverage for  [react-timeago (v3.2.0)](https://github.com/nmn/react-timeago)  [![npm package](https://img.shields.io/npm/v/npmtest-react-timeago.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-react-timeago) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-react-timeago.svg)](https://travis-ci.org/npmtest/node-npmtest-react-timeago)

#### A simple Time-Ago component for ReactJs

[![NPM](https://nodei.co/npm/react-timeago.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-timeago)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-react-timeago/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-timeago/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-react-timeago/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-react-timeago/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-react-timeago/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-react-timeago/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-react-timeago/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-react-timeago/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-react-timeago/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-timeago/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-react-timeago/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-react-timeago/build/test-report.html](https://npmtest.github.io/node-npmtest-react-timeago/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-react-timeago/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-react-timeago/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-react-timeago/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-timeago/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-timeago/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-timeago/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-react-timeago/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-react-timeago/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "react-timeago",
    "version": "3.2.0",
    "description": "A simple Time-Ago component for ReactJs",
    "main": "lib/index.js",
    "scripts": {
        "cpflow": "find ./src -name '*.js' -not -path '*/__*' | while read filepath; do cp $filepath 'echo $filepath | sed 's/\\/src\\//\\/lib\\//g''.flow; done",
        "babel": "babel src/ --out-dir lib/",
        "example": "browserify -t babelify --debug examples/simple/index.js -o examples/simple/bundle.js",
        "build": "npm run babel && npm run cpflow && npm run example",
        "prepublish": "npm run build",
        "test": "ava --require babel-register",
        "coverall": "nyc npm test && nyc report --reporter=text-lcov | coveralls"
    },
    "ava": {
        "babel": "inherit"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/naman34/react-timeago.git"
    },
    "keywords": [
        "React",
        "ReactJS",
        "Time",
        "Ago",
        "TimeAgo",
        "ender"
    ],
    "author": "Naman Goel",
    "license": "MIT",
    "bugs": {
        "url": "https://github.com/nmn/react-timeago/issues"
    },
    "homepage": "https://github.com/nmn/react-timeago",
    "peerDependencies": {
        "react": "^15.0.0"
    },
    "devDependencies": {
        "ava": "^0.16.0",
        "babel-cli": "^6.14.0",
        "babel-eslint": "^6.1.2",
        "babel-plugin-syntax-flow": "^6.13.0",
        "babel-plugin-syntax-jsx": "^6.13.0",
        "babel-plugin-transform-flow-strip-types": "^6.14.0",
        "babel-plugin-transform-react-jsx": "^6.7.5",
        "babel-preset-es2015": "^6.14.0",
        "babel-preset-react": "^6.11.1",
        "babel-preset-stage-1": "^6.13.0",
        "babel-register": "^6.18.0",
        "babelify": "^7.3.0",
        "browserify": "^13.1.0",
        "coveralls": "^2.11.12",
        "enzyme": "^2.4.1",
        "eslint": "^3.4.0",
        "eslint-config-standard": "^6.0.0",
        "eslint-config-standard-react": "^4.0.0",
        "eslint-plugin-flow-vars": "^0.5.0",
        "eslint-plugin-flowtype": "^2.16.0",
        "eslint-plugin-promise": "^2.0.1",
        "eslint-plugin-react": "^6.2.0",
        "eslint-plugin-standard": "^2.0.0",
        "nyc": "^8.0.0",
        "react": "^15.0.0-rc.2",
        "react-addons-test-utils": "^15.3.0",
        "react-dom": "^15.3.1"
    },
    "dependencies": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
