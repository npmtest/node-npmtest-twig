# npmtest-twig

#### basic test coverage for  [twig (v1.10.4)](https://github.com/twigjs/twig.js)  [![npm package](https://img.shields.io/npm/v/npmtest-twig.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-twig) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-twig.svg)](https://travis-ci.org/npmtest/node-npmtest-twig)

#### JS port of the Twig templating language.

[![NPM](https://nodei.co/npm/twig.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/twig)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-twig/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-twig/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-twig/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-twig/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-twig/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-twig/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-twig/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-twig/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-twig/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-twig/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-twig/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-twig/build/test-report.html](https://npmtest.github.io/node-npmtest-twig/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-twig/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-twig/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-twig/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-twig/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-twig/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-twig/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-twig/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-twig/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": "John Roepke <john@justjohn.us> (http://john.sh/)",
    "name": "twig",
    "description": "JS port of the Twig templating language.",
    "version": "1.10.4",
    "homepage": "https://github.com/twigjs/twig.js",
    "licenses": [
        {
            "type": "BSD-2-Clause",
            "url": "https://raw.github.com/twigjs/twig.js/master/LICENSE"
        }
    ],
    "repository": {
        "type": "git",
        "url": "git://github.com/twigjs/twig.js.git"
    },
    "main": "twig.js",
    "engines": {
        "node": "*"
    },
    "bin": {
        "twigjs": "./bin/twigjs"
    },
    "scripts": {
        "preversion": "npm test && git diff --exit-code --quiet",
        "postversion": "git push origin master && git push origin master --tags",
        "test": "npm run build && mocha -r should",
        "build-node": "webpack",
        "build-browser": "WEBPACK_ENV=browser webpack",
        "build": "npm run build-node && npm run build-browser"
    },
    "dependencies": {
        "minimatch": "3.0.x",
        "locutus": "^2.0.5",
        "walk": "2.3.x"
    },
    "devDependencies": {
        "chai": "^3.5.0",
        "mocha": "3.1.x",
        "should": "11.1.x",
        "sinon": "^1.17.6",
        "sinon-chai": "^2.8.0",
        "tokenizer": "1.1.x",
        "webpack": "^1.13.3"
    },
    "browser": {
        "fs": false
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
