# npmdoc-google-libphonenumber

#### api documentation for  [google-libphonenumber (v2.0.15)](http://seegno.github.io/google-libphonenumber/)  [![npm package](https://img.shields.io/npm/v/npmdoc-google-libphonenumber.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-google-libphonenumber) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-google-libphonenumber.svg)](https://travis-ci.org/npmdoc/node-npmdoc-google-libphonenumber)

#### The up-to-date and reliable Google's libphonenumber package for node.js.

[![NPM](https://nodei.co/npm/google-libphonenumber.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/google-libphonenumber)

- [https://npmdoc.github.io/node-npmdoc-google-libphonenumber/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-google-libphonenumber/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-google-libphonenumber/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-google-libphonenumber/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-google-libphonenumber/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-google-libphonenumber/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Rui Marinho",
        "url": "http://seegno.com"
    },
    "bugs": {
        "url": "https://github.com/seegno/google-libphonenumber/issues"
    },
    "dependencies": {},
    "description": "The up-to-date and reliable Google's libphonenumber package for node.js.",
    "devDependencies": {
        "browserify": "^13.1.0",
        "eslint": "^3.5.0",
        "eslint-config-seegno": "^6.0.0",
        "mocha": "^3.0.2",
        "should": "^11.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "d890959d2f7e374ff901296bc76d07f1e24adabe",
        "tarball": "https://registry.npmjs.org/google-libphonenumber/-/google-libphonenumber-2.0.15.tgz"
    },
    "engines": {
        "node": ">=0.10"
    },
    "gitHead": "7e88e7f5bcb031488e2438c48c722f1f70bec5d3",
    "homepage": "http://seegno.github.io/google-libphonenumber/",
    "keywords": [
        "browserify",
        "e164",
        "format",
        "formatting",
        "international",
        "libphonenumber",
        "number",
        "phone",
        "phonenumber",
        "rfc3966",
        "standardize",
        "wrapper"
    ],
    "license": "SEE LICENSE IN LICENSE",
    "main": "dist/libphonenumber.js",
    "maintainers": [
        {
            "name": "ruimarinho"
        }
    ],
    "name": "google-libphonenumber",
    "optionalDependencies": {},
    "options": {
        "mocha": "--require should test"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/seegno/google-libphonenumber.git"
    },
    "scripts": {
        "build": "bin/build.sh",
        "changelog": "github_changelog_generator --no-issues --header-label='# Changelog' --future-release=v$npm_config_future_release && sed -i '' -e :a -e '$d;N;2,3ba' -e 'P;D' CHANGELOG.md",
        "lint": "eslint src/index.js test",
        "prepublish": "npm run build",
        "test": "npm run build && npm run testonly",
        "testonly": "mocha $npm_package_options_mocha",
        "update": "bin/update.sh",
        "version": "npm run changelog --future-release=$npm_package_version && npm run build && git add -A CHANGELOG.md dist"
    },
    "version": "2.0.15"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
