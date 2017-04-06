# api documentation for  [google-libphonenumber (v2.0.14)](http://seegno.github.io/google-libphonenumber/)  [![npm package](https://img.shields.io/npm/v/npmdoc-google-libphonenumber.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-google-libphonenumber) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-google-libphonenumber.svg)](https://travis-ci.org/npmdoc/node-npmdoc-google-libphonenumber)
#### The up-to-date and reliable Google's libphonenumber package for node.js.

[![NPM](https://nodei.co/npm/google-libphonenumber.png?downloads=true)](https://www.npmjs.com/package/google-libphonenumber)

[![apidoc](https://npmdoc.github.io/node-npmdoc-google-libphonenumber/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-google-libphonenumber_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-google-libphonenumber/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-google-libphonenumber/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-google-libphonenumber/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Rui Marinho",
        "email": "rui.marinho@seegno.com",
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
        "shasum": "c7496aceb9fc4c7d47c6148985da881814fddd2e",
        "tarball": "https://registry.npmjs.org/google-libphonenumber/-/google-libphonenumber-2.0.14.tgz"
    },
    "engines": {
        "node": ">=0.10"
    },
    "gitHead": "0bc7603296b599dd4c00738bba942a0a5bf22c1c",
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
            "name": "ruimarinho",
            "email": "ruipmarinho@gmail.com"
        }
    ],
    "name": "google-libphonenumber",
    "optionalDependencies": {},
    "options": {
        "mocha": "--require should test"
    },
    "readme": "ERROR: No README data found!",
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
    "version": "2.0.14"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module google-libphonenumber](#apidoc.module.google-libphonenumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.</span>AsYouTypeFormatter (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.</span>NumberFormat ()](#apidoc.element.google-libphonenumber.NumberFormat)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneMetadata ()](#apidoc.element.google-libphonenumber.PhoneMetadata)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneMetadataCollection ()](#apidoc.element.google-libphonenumber.PhoneMetadataCollection)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneNumber ()](#apidoc.element.google-libphonenumber.PhoneNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneNumberDesc ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneNumberUtil ()](#apidoc.element.google-libphonenumber.PhoneNumberUtil)
1.  object <span class="apidocSignatureSpan">google-libphonenumber.</span>AsYouTypeFormatter.prototype
1.  object <span class="apidocSignatureSpan">google-libphonenumber.</span>Error
1.  object <span class="apidocSignatureSpan">google-libphonenumber.</span>NumberFormat.prototype
1.  object <span class="apidocSignatureSpan">google-libphonenumber.</span>NumberFormat.superClass_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneMetadata.descriptor_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneMetadata.prototype
1.  object <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneMetadataCollection.prototype
1.  object <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneNumber.prototype
1.  object <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneNumberDesc.prototype
1.  object <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneNumberFormat
1.  object <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneNumberType
1.  object <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneNumberUtil.prototype
1.  object <span class="apidocSignatureSpan">google-libphonenumber.</span>metadata

#### [module google-libphonenumber.AsYouTypeFormatter](#apidoc.module.google-libphonenumber.AsYouTypeFormatter)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.</span>AsYouTypeFormatter (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.AsYouTypeFormatter)
1.  number <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.</span>MIN_LEADING_DIGITS_LENGTH_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.</span>CHARACTER_CLASS_PATTERN_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.</span>ELIGIBLE_FORMAT_PATTERN_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.</span>EMPTY_METADATA_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.</span>NATIONAL_PREFIX_SEPARATORS_PATTERN_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.</span>STANDALONE_DIGIT_PATTERN_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.</span>SEPARATOR_BEFORE_NATIONAL_NUMBER_

#### [module google-libphonenumber.AsYouTypeFormatter.prototype](#apidoc.module.google-libphonenumber.AsYouTypeFormatter.prototype)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>ableToExtractLongerNdd_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.ableToExtractLongerNdd_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>appendNationalNumber_ (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.appendNationalNumber_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>attemptToChooseFormattingPattern_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.attemptToChooseFormattingPattern_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>attemptToChoosePatternWithPrefixExtracted_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.attemptToChoosePatternWithPrefixExtracted_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>attemptToExtractCountryCallingCode_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.attemptToExtractCountryCallingCode_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>attemptToExtractIdd_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.attemptToExtractIdd_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>attemptToFormatAccruedDigits_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.attemptToFormatAccruedDigits_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>clear ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.clear)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>createFormattingTemplate_ (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.createFormattingTemplate_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>getAvailableFormats_ (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.getAvailableFormats_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>getExtractedNationalPrefix_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.getExtractedNationalPrefix_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>getFormattingTemplate_ (a, b)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.getFormattingTemplate_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>getMetadataForRegion_ (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.getMetadataForRegion_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>getRememberedPosition ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.getRememberedPosition)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>inputAccruedNationalNumber_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.inputAccruedNationalNumber_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>inputDigit (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.inputDigit)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>inputDigitAndRememberPosition (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.inputDigitAndRememberPosition)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>inputDigitHelper_ (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.inputDigitHelper_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>inputDigitWithOptionToRememberPosition_ (a, b)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.inputDigitWithOptionToRememberPosition_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>isDigitOrLeadingPlusSign_ (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.isDigitOrLeadingPlusSign_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>isFormatEligible_ (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.isFormatEligible_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>isNanpaNumberWithNationalPrefix_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.isNanpaNumberWithNationalPrefix_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>maybeCreateNewTemplate_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.maybeCreateNewTemplate_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>narrowDownPossibleFormats_ (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.narrowDownPossibleFormats_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>normalizeAndAccrueDigitsAndPlusSign_ (a, b)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.normalizeAndAccrueDigitsAndPlusSign_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>removeNationalPrefixFromNationalNumber_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.removeNationalPrefixFromNationalNumber_)

#### [module google-libphonenumber.NumberFormat](#apidoc.module.google-libphonenumber.NumberFormat)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.</span>NumberFormat ()](#apidoc.element.google-libphonenumber.NumberFormat.NumberFormat)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.</span>base (a, c, f)](#apidoc.element.google-libphonenumber.NumberFormat.base)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.NumberFormat.getDescriptor)
1.  object <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.</span>descriptor_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.</span>superClass_

#### [module google-libphonenumber.NumberFormat.prototype](#apidoc.module.google-libphonenumber.NumberFormat.prototype)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>addLeadingDigitsPattern (a)](#apidoc.element.google-libphonenumber.NumberFormat.prototype.addLeadingDigitsPattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>clearDomesticCarrierCodeFormattingRule ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.clearDomesticCarrierCodeFormattingRule)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>clearFormat ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.clearFormat)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>clearLeadingDigitsPattern ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.clearLeadingDigitsPattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>clearNationalPrefixFormattingRule ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.clearNationalPrefixFormattingRule)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>clearNationalPrefixOptionalWhenFormatting ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.clearNationalPrefixOptionalWhenFormatting)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>clearPattern ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.clearPattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>constructor ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>domesticCarrierCodeFormattingRuleCount ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.domesticCarrierCodeFormattingRuleCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>formatCount ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.formatCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getDescriptor)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getDomesticCarrierCodeFormattingRule ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getDomesticCarrierCodeFormattingRule)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getDomesticCarrierCodeFormattingRuleOrDefault ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getDomesticCarrierCodeFormattingRuleOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getFormat ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getFormat)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getFormatOrDefault ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getFormatOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getLeadingDigitsPattern (a)](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getLeadingDigitsPattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getLeadingDigitsPatternOrDefault (a)](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getLeadingDigitsPatternOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getNationalPrefixFormattingRule ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getNationalPrefixFormattingRule)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getNationalPrefixFormattingRuleOrDefault ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getNationalPrefixFormattingRuleOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getNationalPrefixOptionalWhenFormatting ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getNationalPrefixOptionalWhenFormatting)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getNationalPrefixOptionalWhenFormattingOrDefault ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getNationalPrefixOptionalWhenFormattingOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getPattern ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getPattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getPatternOrDefault ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getPatternOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>hasDomesticCarrierCodeFormattingRule ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.hasDomesticCarrierCodeFormattingRule)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>hasFormat ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.hasFormat)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>hasLeadingDigitsPattern ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.hasLeadingDigitsPattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>hasNationalPrefixFormattingRule ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.hasNationalPrefixFormattingRule)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>hasNationalPrefixOptionalWhenFormatting ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.hasNationalPrefixOptionalWhenFormatting)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>hasPattern ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.hasPattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>leadingDigitsPatternArray ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.leadingDigitsPatternArray)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>leadingDigitsPatternCount ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.leadingDigitsPatternCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>nationalPrefixFormattingRuleCount ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.nationalPrefixFormattingRuleCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>nationalPrefixOptionalWhenFormattingCount ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.nationalPrefixOptionalWhenFormattingCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>patternCount ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.patternCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>setDomesticCarrierCodeFormattingRule (a)](#apidoc.element.google-libphonenumber.NumberFormat.prototype.setDomesticCarrierCodeFormattingRule)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>setFormat (a)](#apidoc.element.google-libphonenumber.NumberFormat.prototype.setFormat)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>setNationalPrefixFormattingRule (a)](#apidoc.element.google-libphonenumber.NumberFormat.prototype.setNationalPrefixFormattingRule)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>setNationalPrefixOptionalWhenFormatting (a)](#apidoc.element.google-libphonenumber.NumberFormat.prototype.setNationalPrefixOptionalWhenFormatting)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>setPattern (a)](#apidoc.element.google-libphonenumber.NumberFormat.prototype.setPattern)

#### [module google-libphonenumber.NumberFormat.superClass_](#apidoc.module.google-libphonenumber.NumberFormat.superClass_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>add (a, b)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.add)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>arrayOf (a)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.arrayOf)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>checkFieldType_ (a, b)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.checkFieldType_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>clear (a)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.clear)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>clone ()](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.clone)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>copyFrom (a)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.copyFrom)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>countOf (a)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.countOf)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>equals (a)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.equals)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>forEachUnknown (a, b)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.forEachUnknown)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>get (a, b)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.get)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.getDescriptor)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>getOrDefault (a, b)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.getOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>getValueForTag_ (a)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.getValueForTag_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>has (a)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.has)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>initDefaults (a)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.initDefaults)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>initializeForLazyDeserializer (a, b)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.initializeForLazyDeserializer)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>mergeFrom (a)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.mergeFrom)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>set (a, b)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.set)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>setUnknown (a, b)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.setUnknown)

#### [module google-libphonenumber.PhoneMetadata](#apidoc.module.google-libphonenumber.PhoneMetadata)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneMetadata ()](#apidoc.element.google-libphonenumber.PhoneMetadata.PhoneMetadata)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.</span>base (a, c, f)](#apidoc.element.google-libphonenumber.PhoneMetadata.base)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.PhoneMetadata.getDescriptor)
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.</span>descriptor_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.</span>superClass_

#### [module google-libphonenumber.PhoneMetadata.descriptor_](#apidoc.module.google-libphonenumber.PhoneMetadata.descriptor_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.descriptor_.</span>messageType_ ()](#apidoc.element.google-libphonenumber.PhoneMetadata.descriptor_.messageType_)
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.descriptor_.</span>fields_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.descriptor_.</span>fullName_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.descriptor_.</span>name_

#### [module google-libphonenumber.PhoneMetadata.prototype](#apidoc.module.google-libphonenumber.PhoneMetadata.prototype)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>addIntlNumberFormat (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.addIntlNumberFormat)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>addNumberFormat (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.addNumberFormat)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearCountryCode ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearCountryCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearEmergency ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearEmergency)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearFixedLine ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearFixedLine)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearGeneralDesc ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearGeneralDesc)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearId ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearId)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearInternationalPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearInternationalPrefix)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearIntlNumberFormat ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearIntlNumberFormat)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearLeadingDigits ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearLeadingDigits)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearLeadingZeroPossible ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearLeadingZeroPossible)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearMainCountryForCode ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearMainCountryForCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearMobile ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearMobile)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearNationalPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearNationalPrefix)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearNationalPrefixForParsing ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearNationalPrefixForParsing)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearNationalPrefixTransformRule ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearNationalPrefixTransformRule)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearNoInternationalDialling ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearNoInternationalDialling)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearNumberFormat ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearNumberFormat)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearPager ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearPager)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearPersonalNumber ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearPersonalNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearPreferredExtnPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearPreferredExtnPrefix)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearPreferredInternationalPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearPreferredInternationalPrefix)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearPremiumRate ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearPremiumRate)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearSameMobileAndFixedLinePattern ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearSameMobileAndFixedLinePattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearSharedCost ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearSharedCost)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearTollFree ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearTollFree)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearUan ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearUan)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearVoicemail ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearVoicemail)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearVoip ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearVoip)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>constructor ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>countryCodeCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.countryCodeCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>emergencyCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.emergencyCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>fixedLineCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.fixedLineCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>generalDescCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.generalDescCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getCountryCode ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getCountryCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getCountryCodeOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getCountryCodeOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getDescriptor)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getEmergency ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getEmergency)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getEmergencyOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getEmergencyOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getFixedLine ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getFixedLine)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getFixedLineOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getFixedLineOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getGeneralDesc ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getGeneralDesc)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getGeneralDescOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getGeneralDescOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getId ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getId)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getIdOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getIdOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getInternationalPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getInternationalPrefix)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getInternationalPrefixOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getInternationalPrefixOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getIntlNumberFormat (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getIntlNumberFormat)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getIntlNumberFormatOrDefault (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getIntlNumberFormatOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getLeadingDigits ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getLeadingDigits)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getLeadingDigitsOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getLeadingDigitsOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getLeadingZeroPossible ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getLeadingZeroPossible)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getLeadingZeroPossibleOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getLeadingZeroPossibleOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getMainCountryForCode ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getMainCountryForCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getMainCountryForCodeOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getMainCountryForCodeOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getMobile ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getMobile)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getMobileOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getMobileOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNationalPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNationalPrefix)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNationalPrefixForParsing ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNationalPrefixForParsing)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNationalPrefixForParsingOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNationalPrefixForParsingOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNationalPrefixOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNationalPrefixOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNationalPrefixTransformRule ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNationalPrefixTransformRule)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNationalPrefixTransformRuleOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNationalPrefixTransformRuleOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNoInternationalDialling ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNoInternationalDialling)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNoInternationalDiallingOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNoInternationalDiallingOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNumberFormat (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNumberFormat)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNumberFormatOrDefault (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNumberFormatOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPager ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPager)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPagerOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPagerOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPersonalNumber ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPersonalNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPersonalNumberOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPersonalNumberOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPreferredExtnPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPreferredExtnPrefix)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPreferredExtnPrefixOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPreferredExtnPrefixOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPreferredInternationalPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPreferredInternationalPrefix)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPreferredInternationalPrefixOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPreferredInternationalPrefixOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPremiumRate ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPremiumRate)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPremiumRateOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPremiumRateOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getSameMobileAndFixedLinePattern ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getSameMobileAndFixedLinePattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getSameMobileAndFixedLinePatternOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getSameMobileAndFixedLinePatternOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getSharedCost ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getSharedCost)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getSharedCostOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getSharedCostOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getTollFree ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getTollFree)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getTollFreeOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getTollFreeOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getUan ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getUan)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getUanOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getUanOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getVoicemail ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getVoicemail)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getVoicemailOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getVoicemailOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getVoip ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getVoip)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getVoipOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getVoipOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasCountryCode ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasCountryCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasEmergency ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasEmergency)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasFixedLine ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasFixedLine)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasGeneralDesc ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasGeneralDesc)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasId ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasId)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasInternationalPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasInternationalPrefix)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasIntlNumberFormat ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasIntlNumberFormat)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasLeadingDigits ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasLeadingDigits)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasLeadingZeroPossible ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasLeadingZeroPossible)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasMainCountryForCode ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasMainCountryForCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasMobile ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasMobile)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasNationalPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasNationalPrefix)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasNationalPrefixForParsing ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasNationalPrefixForParsing)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasNationalPrefixTransformRule ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasNationalPrefixTransformRule)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasNoInternationalDialling ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasNoInternationalDialling)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasNumberFormat ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasNumberFormat)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasPager ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasPager)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasPersonalNumber ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasPersonalNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasPreferredExtnPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasPreferredExtnPrefix)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasPreferredInternationalPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasPreferredInternationalPrefix)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasPremiumRate ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasPremiumRate)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasSameMobileAndFixedLinePattern ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasSameMobileAndFixedLinePattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasSharedCost ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasSharedCost)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasTollFree ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasTollFree)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasUan ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasUan)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasVoicemail ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasVoicemail)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasVoip ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasVoip)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>idCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.idCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>internationalPrefixCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.internationalPrefixCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>intlNumberFormatArray ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.intlNumberFormatArray)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>intlNumberFormatCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.intlNumberFormatCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>leadingDigitsCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.leadingDigitsCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>leadingZeroPossibleCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.leadingZeroPossibleCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>mainCountryForCodeCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.mainCountryForCodeCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>mobileCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.mobileCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>nationalPrefixCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.nationalPrefixCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>nationalPrefixForParsingCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.nationalPrefixForParsingCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>nationalPrefixTransformRuleCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.nationalPrefixTransformRuleCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>noInternationalDiallingCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.noInternationalDiallingCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>numberFormatArray ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.numberFormatArray)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>numberFormatCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.numberFormatCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>pagerCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.pagerCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>personalNumberCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.personalNumberCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>preferredExtnPrefixCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.preferredExtnPrefixCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>preferredInternationalPrefixCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.preferredInternationalPrefixCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>premiumRateCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.premiumRateCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>sameMobileAndFixedLinePatternCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.sameMobileAndFixedLinePatternCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setCountryCode (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setCountryCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setEmergency (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setEmergency)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setFixedLine (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setFixedLine)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setGeneralDesc (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setGeneralDesc)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setId (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setId)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setInternationalPrefix (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setInternationalPrefix)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setLeadingDigits (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setLeadingDigits)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setLeadingZeroPossible (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setLeadingZeroPossible)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setMainCountryForCode (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setMainCountryForCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setMobile (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setMobile)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setNationalPrefix (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setNationalPrefix)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setNationalPrefixForParsing (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setNationalPrefixForParsing)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setNationalPrefixTransformRule (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setNationalPrefixTransformRule)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setNoInternationalDialling (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setNoInternationalDialling)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setPager (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setPager)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setPersonalNumber (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setPersonalNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setPreferredExtnPrefix (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setPreferredExtnPrefix)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setPreferredInternationalPrefix (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setPreferredInternationalPrefix)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setPremiumRate (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setPremiumRate)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setSameMobileAndFixedLinePattern (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setSameMobileAndFixedLinePattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setSharedCost (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setSharedCost)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setTollFree (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setTollFree)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setUan (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setUan)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setVoicemail (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setVoicemail)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setVoip (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setVoip)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>sharedCostCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.sharedCostCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>tollFreeCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.tollFreeCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>uanCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.uanCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>voicemailCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.voicemailCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>voipCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.voipCount)

#### [module google-libphonenumber.PhoneMetadataCollection](#apidoc.module.google-libphonenumber.PhoneMetadataCollection)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneMetadataCollection ()](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.PhoneMetadataCollection)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.</span>base (a, c, f)](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.base)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.getDescriptor)
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.</span>descriptor_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.</span>superClass_

#### [module google-libphonenumber.PhoneMetadataCollection.prototype](#apidoc.module.google-libphonenumber.PhoneMetadataCollection.prototype)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.prototype.</span>addMetadata (a)](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.addMetadata)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.prototype.</span>clearMetadata ()](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.clearMetadata)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.prototype.</span>constructor ()](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.prototype.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.getDescriptor)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.prototype.</span>getMetadata (a)](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.getMetadata)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.prototype.</span>getMetadataOrDefault (a)](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.getMetadataOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.prototype.</span>hasMetadata ()](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.hasMetadata)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.prototype.</span>metadataArray ()](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.metadataArray)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.prototype.</span>metadataCount ()](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.metadataCount)

#### [module google-libphonenumber.PhoneNumber](#apidoc.module.google-libphonenumber.PhoneNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneNumber ()](#apidoc.element.google-libphonenumber.PhoneNumber.PhoneNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.</span>base (a, c, f)](#apidoc.element.google-libphonenumber.PhoneNumber.base)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.</span>ctor ()](#apidoc.element.google-libphonenumber.PhoneNumber.ctor)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.PhoneNumber.getDescriptor)
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.</span>CountryCodeSource
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.</span>superClass_

#### [module google-libphonenumber.PhoneNumber.prototype](#apidoc.module.google-libphonenumber.PhoneNumber.prototype)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>clearCountryCode ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearCountryCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>clearCountryCodeSource ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearCountryCodeSource)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>clearExtension ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearExtension)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>clearItalianLeadingZero ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearItalianLeadingZero)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>clearNationalNumber ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearNationalNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>clearNumberOfLeadingZeros ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearNumberOfLeadingZeros)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>clearPreferredDomesticCarrierCode ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearPreferredDomesticCarrierCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>clearRawInput ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearRawInput)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>constructor ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>countryCodeCount ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.countryCodeCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>countryCodeSourceCount ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.countryCodeSourceCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>extensionCount ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.extensionCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getCountryCode ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getCountryCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getCountryCodeOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getCountryCodeOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getCountryCodeSource ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getCountryCodeSource)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getCountryCodeSourceOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getCountryCodeSourceOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getDescriptor)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getExtension ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getExtension)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getExtensionOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getExtensionOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getItalianLeadingZero ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getItalianLeadingZero)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getItalianLeadingZeroOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getItalianLeadingZeroOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getNationalNumber ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getNationalNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getNationalNumberOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getNationalNumberOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getNumberOfLeadingZeros ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getNumberOfLeadingZeros)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getNumberOfLeadingZerosOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getNumberOfLeadingZerosOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getPreferredDomesticCarrierCode ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getPreferredDomesticCarrierCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getPreferredDomesticCarrierCodeOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getPreferredDomesticCarrierCodeOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getRawInput ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getRawInput)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getRawInputOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getRawInputOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>hasCountryCode ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasCountryCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>hasCountryCodeSource ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasCountryCodeSource)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>hasExtension ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasExtension)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>hasItalianLeadingZero ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasItalianLeadingZero)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>hasNationalNumber ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasNationalNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>hasNumberOfLeadingZeros ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasNumberOfLeadingZeros)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>hasPreferredDomesticCarrierCode ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasPreferredDomesticCarrierCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>hasRawInput ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasRawInput)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>italianLeadingZeroCount ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.italianLeadingZeroCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>nationalNumberCount ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.nationalNumberCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>numberOfLeadingZerosCount ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.numberOfLeadingZerosCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>preferredDomesticCarrierCodeCount ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.preferredDomesticCarrierCodeCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>rawInputCount ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.rawInputCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>setCountryCode (a)](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.setCountryCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>setCountryCodeSource (a)](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.setCountryCodeSource)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>setExtension (a)](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.setExtension)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>setItalianLeadingZero (a)](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.setItalianLeadingZero)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>setNationalNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.setNationalNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>setNumberOfLeadingZeros (a)](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.setNumberOfLeadingZeros)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>setPreferredDomesticCarrierCode (a)](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.setPreferredDomesticCarrierCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>setRawInput (a)](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.setRawInput)

#### [module google-libphonenumber.PhoneNumberDesc](#apidoc.module.google-libphonenumber.PhoneNumberDesc)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneNumberDesc ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.PhoneNumberDesc)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.</span>base (a, c, f)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.base)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.getDescriptor)
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.</span>descriptor_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.</span>superClass_

#### [module google-libphonenumber.PhoneNumberDesc.prototype](#apidoc.module.google-libphonenumber.PhoneNumberDesc.prototype)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>addPossibleLength (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.addPossibleLength)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>addPossibleLengthLocalOnly (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.addPossibleLengthLocalOnly)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>clearExampleNumber ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearExampleNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>clearNationalNumberMatcherData ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearNationalNumberMatcherData)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>clearNationalNumberPattern ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearNationalNumberPattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>clearPossibleLength ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearPossibleLength)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>clearPossibleLengthLocalOnly ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearPossibleLengthLocalOnly)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>clearPossibleNumberMatcherData ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearPossibleNumberMatcherData)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>clearPossibleNumberPattern ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearPossibleNumberPattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>constructor ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>exampleNumberCount ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.exampleNumberCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getDescriptor)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getExampleNumber ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getExampleNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getExampleNumberOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getExampleNumberOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getNationalNumberMatcherData ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getNationalNumberMatcherData)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getNationalNumberMatcherDataOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getNationalNumberMatcherDataOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getNationalNumberPattern ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getNationalNumberPattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getNationalNumberPatternOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getNationalNumberPatternOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getPossibleLength (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleLength)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getPossibleLengthLocalOnly (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleLengthLocalOnly)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getPossibleLengthLocalOnlyOrDefault (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleLengthLocalOnlyOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getPossibleLengthOrDefault (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleLengthOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getPossibleNumberMatcherData ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleNumberMatcherData)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getPossibleNumberMatcherDataOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleNumberMatcherDataOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getPossibleNumberPattern ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleNumberPattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getPossibleNumberPatternOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleNumberPatternOrDefault)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>hasExampleNumber ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasExampleNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>hasNationalNumberMatcherData ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasNationalNumberMatcherData)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>hasNationalNumberPattern ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasNationalNumberPattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>hasPossibleLength ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasPossibleLength)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>hasPossibleLengthLocalOnly ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasPossibleLengthLocalOnly)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>hasPossibleNumberMatcherData ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasPossibleNumberMatcherData)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>hasPossibleNumberPattern ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasPossibleNumberPattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>nationalNumberMatcherDataCount ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.nationalNumberMatcherDataCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>nationalNumberPatternCount ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.nationalNumberPatternCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>possibleLengthArray ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.possibleLengthArray)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>possibleLengthCount ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.possibleLengthCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>possibleLengthLocalOnlyArray ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.possibleLengthLocalOnlyArray)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>possibleLengthLocalOnlyCount ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.possibleLengthLocalOnlyCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>possibleNumberMatcherDataCount ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.possibleNumberMatcherDataCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>possibleNumberPatternCount ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.possibleNumberPatternCount)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>setExampleNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.setExampleNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>setNationalNumberMatcherData (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.setNationalNumberMatcherData)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>setNationalNumberPattern (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.setNationalNumberPattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>setPossibleNumberMatcherData (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.setPossibleNumberMatcherData)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>setPossibleNumberPattern (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.setPossibleNumberPattern)

#### [module google-libphonenumber.PhoneNumberUtil](#apidoc.module.google-libphonenumber.PhoneNumberUtil)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneNumberUtil ()](#apidoc.element.google-libphonenumber.PhoneNumberUtil.PhoneNumberUtil)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>convertAlphaCharactersInNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.convertAlphaCharactersInNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>copyCoreFieldsOnly_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.copyCoreFieldsOnly_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>descHasData_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.descHasData_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>descHasPossibleNumberData_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.descHasPossibleNumberData_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>extractPossibleNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.extractPossibleNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>getCountryMobileToken (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.getCountryMobileToken)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>getInstance ()](#apidoc.element.google-libphonenumber.PhoneNumberUtil.getInstance)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>getNumberDescByType_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.getNumberDescByType_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>getSupportedTypesForMetadata_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.getSupportedTypesForMetadata_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>isViablePhoneNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.isViablePhoneNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>matchesEntirely_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.matchesEntirely_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>normalize (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.normalize)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>normalizeDiallableCharsOnly (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.normalizeDiallableCharsOnly)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>normalizeDigitsOnly (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.normalizeDigitsOnly)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>normalizeHelper_ (a, b, c)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.normalizeHelper_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>normalizeSB_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.normalizeSB_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>setItalianLeadingZerosForPhoneNumber_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.setItalianLeadingZerosForPhoneNumber_)
1.  number <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>MAX_INPUT_STRING_LENGTH_
1.  number <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>MAX_LENGTH_COUNTRY_CODE_
1.  number <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>MAX_LENGTH_FOR_NSN_
1.  number <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>MIN_LENGTH_FOR_NSN_
1.  number <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>NANPA_COUNTRY_CODE_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>ALL_NORMALIZATION_MAPPINGS_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>ALL_PLUS_NUMBER_GROUPING_SYMBOLS_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>ALPHA_MAPPINGS_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>CAPTURING_DIGIT_PATTERN
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>CC_PATTERN_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>DIALLABLE_CHAR_MAPPINGS_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>DIGIT_MAPPINGS
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>EXTN_PATTERN_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>FG_PATTERN_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>FIRST_GROUP_ONLY_PREFIX_PATTERN_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>FIRST_GROUP_PATTERN_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>GEO_MOBILE_COUNTRIES_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>LEADING_PLUS_CHARS_PATTERN_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>MOBILE_TOKEN_MAPPINGS_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>MatchType
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>NON_DIGITS_PATTERN_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>NP_PATTERN_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>PLUS_CHARS_PATTERN
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>SECOND_NUMBER_START_PATTERN_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>UNIQUE_INTERNATIONAL_PREFIX_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>UNWANTED_END_CHAR_PATTERN_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>VALID_ALPHA_PHONE_PATTERN_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>VALID_PHONE_NUMBER_PATTERN_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>VALID_START_CHAR_PATTERN_
1.  object <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>ValidationResult
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>CAPTURING_EXTN_DIGITS_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>COLOMBIA_MOBILE_TO_FIXED_LINE_PREFIX_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>DEFAULT_EXTN_PREFIX_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>EXTN_PATTERNS_FOR_PARSING_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>MIN_LENGTH_PHONE_NUMBER_PATTERN_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>PLUS_CHARS_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>PLUS_SIGN
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>REGION_CODE_FOR_NON_GEO_ENTITY
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>RFC3966_EXTN_PREFIX_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>RFC3966_ISDN_SUBADDRESS_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>RFC3966_PHONE_CONTEXT_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>RFC3966_PREFIX_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>SEPARATOR_PATTERN_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>STAR_SIGN_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>UNKNOWN_REGION_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>VALID_ALPHA_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>VALID_DIGITS_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>VALID_PHONE_NUMBER_
1.  string <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>VALID_PUNCTUATION

#### [module google-libphonenumber.PhoneNumberUtil.prototype](#apidoc.module.google-libphonenumber.PhoneNumberUtil.prototype)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>buildNationalNumberForParsing_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.buildNationalNumberForParsing_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>canBeInternationallyDialled (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.canBeInternationallyDialled)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>checkRegionForParsing_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.checkRegionForParsing_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>chooseFormattingPatternForNumber_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.chooseFormattingPatternForNumber_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>extractCountryCode (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.extractCountryCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>format (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.format)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formatByPattern (a, b, c)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatByPattern)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formatInOriginalFormat (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatInOriginalFormat)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formatNationalNumberWithCarrierCode (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatNationalNumberWithCarrierCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formatNationalNumberWithPreferredCarrierCode (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatNationalNumberWithPreferredCarrierCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formatNsnUsingPattern_ (a, b, c, d)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatNsnUsingPattern_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formatNsn_ (a, b, c, d)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatNsn_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formatNumberForMobileDialing (a, b, c)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatNumberForMobileDialing)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formatOutOfCountryCallingNumber (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatOutOfCountryCallingNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formatOutOfCountryKeepingAlphaChars (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatOutOfCountryKeepingAlphaChars)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formattingRuleHasFirstGroupOnly (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formattingRuleHasFirstGroupOnly)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getCountryCodeForRegion (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getCountryCodeForRegion)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getCountryCodeForValidRegion_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getCountryCodeForValidRegion_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getExampleNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getExampleNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getExampleNumberForNonGeoEntity (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getExampleNumberForNonGeoEntity)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getExampleNumberForType (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getExampleNumberForType)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getLengthOfGeographicalAreaCode (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getLengthOfGeographicalAreaCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getLengthOfNationalDestinationCode (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getLengthOfNationalDestinationCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getMetadataForNonGeographicalRegion (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getMetadataForNonGeographicalRegion)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getMetadataForRegion (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getMetadataForRegion)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getMetadataForRegionOrCallingCode_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getMetadataForRegionOrCallingCode_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getNationalSignificantNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getNationalSignificantNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getNddPrefixForRegion (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getNddPrefixForRegion)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getNumberType (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getNumberType)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getNumberTypeHelper_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getNumberTypeHelper_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getRegionCodeForCountryCode (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getRegionCodeForCountryCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getRegionCodeForNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getRegionCodeForNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getRegionCodeForNumberFromRegionList_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getRegionCodeForNumberFromRegionList_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getRegionCodesForCountryCode (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getRegionCodesForCountryCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getSupportedGlobalNetworkCallingCodes ()](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getSupportedGlobalNetworkCallingCodes)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getSupportedRegions ()](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getSupportedRegions)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getSupportedTypesForNonGeoEntity (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getSupportedTypesForNonGeoEntity)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getSupportedTypesForRegion (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getSupportedTypesForRegion)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>hasFormattingPatternForNumber_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.hasFormattingPatternForNumber_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>hasUnexpectedItalianLeadingZero_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.hasUnexpectedItalianLeadingZero_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>hasValidCountryCallingCode_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.hasValidCountryCallingCode_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isAlphaNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isAlphaNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isLeadingZeroPossible (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isLeadingZeroPossible)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isNANPACountry (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isNANPACountry)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isNationalNumberSuffixOfTheOther_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isNationalNumberSuffixOfTheOther_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isNumberGeographical (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isNumberGeographical)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isNumberMatch (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isNumberMatch)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isNumberMatchingDesc_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isNumberMatchingDesc_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isPossibleNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isPossibleNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isPossibleNumberForType (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isPossibleNumberForType)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isPossibleNumberForTypeWithReason (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isPossibleNumberForTypeWithReason)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isPossibleNumberString (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isPossibleNumberString)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isPossibleNumberWithReason (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isPossibleNumberWithReason)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isValidNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isValidNumber)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isValidNumberForRegion (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isValidNumberForRegion)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isValidRegionCode_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isValidRegionCode_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>maybeExtractCountryCode (a, b, c, d, e)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.maybeExtractCountryCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>maybeGetFormattedExtension_ (a, b, c)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.maybeGetFormattedExtension_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>maybeStripExtension (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.maybeStripExtension)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>maybeStripInternationalPrefixAndNormalize (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.maybeStripInternationalPrefixAndNormalize)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>maybeStripNationalPrefixAndCarrierCode (a, b, c)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.maybeStripNationalPrefixAndCarrierCode)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>parse (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.parse)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>parseAndKeepRawInput (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.parseAndKeepRawInput)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>parseHelper_ (a, b, c, d)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.parseHelper_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>parsePrefixAsIdd_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.parsePrefixAsIdd_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>prefixNumberWithCountryCallingCode_ (a, b, c, d)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.prefixNumberWithCountryCallingCode_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>rawInputContainsNationalPrefix_ (a, b, c)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.rawInputContainsNationalPrefix_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>testNumberLengthForType_ (a, b, c)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.testNumberLengthForType_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>testNumberLength_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.testNumberLength_)
1.  [function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>truncateTooLongNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.truncateTooLongNumber)



# <a name="apidoc.module.google-libphonenumber"></a>[module google-libphonenumber](#apidoc.module.google-libphonenumber)

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.</span>AsYouTypeFormatter (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter)
- description and source-code
```javascript
AsYouTypeFormatter = function (a) {
  this.DIGIT_PLACEHOLDER_ = "\u2008";
  this.DIGIT_PATTERN_ = new RegExp(this.DIGIT_PLACEHOLDER_);
  this.currentOutput_ = "";
  this.formattingTemplate_ = new goog.string.StringBuffer;
  this.currentFormattingPattern_ = "";
  this.accruedInput_ = new goog.string.StringBuffer;
  this.accruedInputWithoutFormatting_ = new goog.string.StringBuffer;
  this.ableToFormat_ = !0;
  this.isExpectingCountryCallingCode_ = this.isCompleteNumber_ = this.inputHasFormatting_ = !1;
  this.phoneUtil_ = i18n.phonenumbers.PhoneNumberUtil.getInstance();
  this.positionToRemember_ = this.originalPosition_ = this.lastMatchPosition_ = 0;
  this.prefixBeforeNationalNumber_ = new goog.string.StringBuffer;
  this.shouldAddSpaceAfterNationalPrefix_ = !1;
  this.extractedNationalPrefix_ = "";
  this.nationalNumber_ = new goog.string.StringBuffer;
  this.possibleFormats_ = [];
  this.defaultCountry_ = a;
  this.defaultMetadata_ = this.currentMetadata_ = this.getMetadataForRegion_(this.defaultCountry_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.</span>NumberFormat ()](#apidoc.element.google-libphonenumber.NumberFormat)
- description and source-code
```javascript
NumberFormat = function () {
  goog.proto2.Message.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneMetadata ()](#apidoc.element.google-libphonenumber.PhoneMetadata)
- description and source-code
```javascript
PhoneMetadata = function () {
  goog.proto2.Message.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadataCollection"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneMetadataCollection ()](#apidoc.element.google-libphonenumber.PhoneMetadataCollection)
- description and source-code
```javascript
PhoneMetadataCollection = function () {
  goog.proto2.Message.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneNumber ()](#apidoc.element.google-libphonenumber.PhoneNumber)
- description and source-code
```javascript
PhoneNumber = function () {
  goog.proto2.Message.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneNumberDesc ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc)
- description and source-code
```javascript
PhoneNumberDesc = function () {
  goog.proto2.Message.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneNumberUtil ()](#apidoc.element.google-libphonenumber.PhoneNumberUtil)
- description and source-code
```javascript
PhoneNumberUtil = function () {
  this.regionToMetadataMap = {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.google-libphonenumber.AsYouTypeFormatter"></a>[module google-libphonenumber.AsYouTypeFormatter](#apidoc.module.google-libphonenumber.AsYouTypeFormatter)

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.AsYouTypeFormatter"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.</span>AsYouTypeFormatter (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.AsYouTypeFormatter)
- description and source-code
```javascript
AsYouTypeFormatter = function (a) {
  this.DIGIT_PLACEHOLDER_ = "\u2008";
  this.DIGIT_PATTERN_ = new RegExp(this.DIGIT_PLACEHOLDER_);
  this.currentOutput_ = "";
  this.formattingTemplate_ = new goog.string.StringBuffer;
  this.currentFormattingPattern_ = "";
  this.accruedInput_ = new goog.string.StringBuffer;
  this.accruedInputWithoutFormatting_ = new goog.string.StringBuffer;
  this.ableToFormat_ = !0;
  this.isExpectingCountryCallingCode_ = this.isCompleteNumber_ = this.inputHasFormatting_ = !1;
  this.phoneUtil_ = i18n.phonenumbers.PhoneNumberUtil.getInstance();
  this.positionToRemember_ = this.originalPosition_ = this.lastMatchPosition_ = 0;
  this.prefixBeforeNationalNumber_ = new goog.string.StringBuffer;
  this.shouldAddSpaceAfterNationalPrefix_ = !1;
  this.extractedNationalPrefix_ = "";
  this.nationalNumber_ = new goog.string.StringBuffer;
  this.possibleFormats_ = [];
  this.defaultCountry_ = a;
  this.defaultMetadata_ = this.currentMetadata_ = this.getMetadataForRegion_(this.defaultCountry_);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.google-libphonenumber.AsYouTypeFormatter.prototype"></a>[module google-libphonenumber.AsYouTypeFormatter.prototype](#apidoc.module.google-libphonenumber.AsYouTypeFormatter.prototype)

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.ableToExtractLongerNdd_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>ableToExtractLongerNdd_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.ableToExtractLongerNdd_)
- description and source-code
```javascript
ableToExtractLongerNdd_ = function () {
  if (0 < this.extractedNationalPrefix_.length) {
    var a = this.nationalNumber_.toString();
    this.nationalNumber_.clear();
    this.nationalNumber_.append(this.extractedNationalPrefix_);
    this.nationalNumber_.append(a);
    var a = this.prefixBeforeNationalNumber_.toString(), b = a.lastIndexOf(this.extractedNationalPrefix_);
    this.prefixBeforeNationalNumber_.clear();
    this.prefixBeforeNationalNumber_.append(a.substring(0, b));
  }
  return this.extractedNationalPrefix_ != this.removeNationalPrefixFromNationalNumber_();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.appendNationalNumber_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>appendNationalNumber_ (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.appendNationalNumber_)
- description and source-code
```javascript
appendNationalNumber_ = function (a) {
  var b = this.prefixBeforeNationalNumber_.getLength();
  return this.shouldAddSpaceAfterNationalPrefix_ && 0 < b && this.prefixBeforeNationalNumber_.toString().charAt(b - 1) != i18n.phonenumbers
.AsYouTypeFormatter.SEPARATOR_BEFORE_NATIONAL_NUMBER_ ? this.prefixBeforeNationalNumber_ + i18n.phonenumbers.AsYouTypeFormatter.
SEPARATOR_BEFORE_NATIONAL_NUMBER_ + a : this.prefixBeforeNationalNumber_ + a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.attemptToChooseFormattingPattern_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>attemptToChooseFormattingPattern_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.attemptToChooseFormattingPattern_)
- description and source-code
```javascript
attemptToChooseFormattingPattern_ = function () {
  var a = this.nationalNumber_.toString();
  return a.length >= i18n.phonenumbers.AsYouTypeFormatter.MIN_LEADING_DIGITS_LENGTH_ ? (this.getAvailableFormats_(a), a = this.attemptToFormatAccruedDigits_
(), 0 < a.length ? a : this.maybeCreateNewTemplate_() ? this.inputAccruedNationalNumber_() : this.accruedInput_.toString()) : this
.appendNationalNumber_(a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.attemptToChoosePatternWithPrefixExtracted_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>attemptToChoosePatternWithPrefixExtracted_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.attemptToChoosePatternWithPrefixExtracted_)
- description and source-code
```javascript
attemptToChoosePatternWithPrefixExtracted_ = function () {
  this.ableToFormat_ = !0;
  this.isExpectingCountryCallingCode_ = !1;
  this.possibleFormats_ = [];
  this.lastMatchPosition_ = 0;
  this.formattingTemplate_.clear();
  this.currentFormattingPattern_ = "";
  return this.attemptToChooseFormattingPattern_();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.attemptToExtractCountryCallingCode_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>attemptToExtractCountryCallingCode_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.attemptToExtractCountryCallingCode_)
- description and source-code
```javascript
attemptToExtractCountryCallingCode_ = function () {
  if (0 == this.nationalNumber_.getLength()) {
    return !1;
  }
  var a = new goog.string.StringBuffer, b = this.phoneUtil_.extractCountryCode(this.nationalNumber_, a);
  if (0 == b) {
    return !1;
  }
  this.nationalNumber_.clear();
  this.nationalNumber_.append(a.toString());
  a = this.phoneUtil_.getRegionCodeForCountryCode(b);
  i18n.phonenumbers.PhoneNumberUtil.REGION_CODE_FOR_NON_GEO_ENTITY == a ? this.currentMetadata_ = this.phoneUtil_.getMetadataForNonGeographicalRegion
(b) : a != this.defaultCountry_ && (this.currentMetadata_ = this.getMetadataForRegion_(a));
  this.prefixBeforeNationalNumber_.append("" + b).append(i18n.phonenumbers.AsYouTypeFormatter.SEPARATOR_BEFORE_NATIONAL_NUMBER_);
  this.extractedNationalPrefix_ = "";
  return !0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.attemptToExtractIdd_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>attemptToExtractIdd_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.attemptToExtractIdd_)
- description and source-code
```javascript
attemptToExtractIdd_ = function () {
  var a = this.accruedInputWithoutFormatting_.toString(), b = new RegExp("^(?:\\" + i18n.phonenumbers.PhoneNumberUtil.PLUS_SIGN + "|" +
this.currentMetadata_.getInternationalPrefix() + ")"), b = a.match(b);
  return null != b && null != b[0] && 0 < b[0].length ? (this.isCompleteNumber_ = !0, b = b[0].length, this.nationalNumber_.clear
(), this.nationalNumber_.append(a.substring(b)), this.prefixBeforeNationalNumber_.clear(), this.prefixBeforeNationalNumber_.append
(a.substring(0, b)), a.charAt(0) != i18n.phonenumbers.PhoneNumberUtil.PLUS_SIGN && this.prefixBeforeNationalNumber_.append(i18n.
phonenumbers.AsYouTypeFormatter.SEPARATOR_BEFORE_NATIONAL_NUMBER_), !0) : !1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.attemptToFormatAccruedDigits_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>attemptToFormatAccruedDigits_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.attemptToFormatAccruedDigits_)
- description and source-code
```javascript
attemptToFormatAccruedDigits_ = function () {
  for (var a = this.nationalNumber_.toString(), b = this.possibleFormats_.length, c = 0;c < b;++c) {
    var d = this.possibleFormats_[c], e = d.getPatternOrDefault();
    if ((new RegExp("^(?:" + e + ")$")).test(a)) {
      return this.shouldAddSpaceAfterNationalPrefix_ = i18n.phonenumbers.AsYouTypeFormatter.NATIONAL_PREFIX_SEPARATORS_PATTERN_.
test(d.getNationalPrefixFormattingRule()), a = a.replace(new RegExp(e, "g"), d.getFormat()), this.appendNationalNumber_(a);
    }
  }
  return "";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.clear"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>clear ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.clear)
- description and source-code
```javascript
clear = function () {
  this.currentOutput_ = "";
  this.accruedInput_.clear();
  this.accruedInputWithoutFormatting_.clear();
  this.formattingTemplate_.clear();
  this.lastMatchPosition_ = 0;
  this.currentFormattingPattern_ = "";
  this.prefixBeforeNationalNumber_.clear();
  this.extractedNationalPrefix_ = "";
  this.nationalNumber_.clear();
  this.ableToFormat_ = !0;
  this.inputHasFormatting_ = !1;
  this.originalPosition_ = this.positionToRemember_ = 0;
  this.isExpectingCountryCallingCode_ = this.isCompleteNumber_ = !1;
  this.possibleFormats_ = [];
  this.shouldAddSpaceAfterNationalPrefix_ = !1;
  this.currentMetadata_ != this.defaultMetadata_ && (this.currentMetadata_ = this.getMetadataForRegion_(this.defaultCountry_));
}
```
- example usage
```shell
...
console.log(formatter.inputDigit('0')); // => 650
console.log(formatter.inputDigit('2')); // => 650-2
console.log(formatter.inputDigit('5')); // => 650-25
console.log(formatter.inputDigit('3')); // => 650-253
console.log(formatter.inputDigit('2')); // => 650-2532
console.log(formatter.inputDigit('2')); // => (650) 253-22

formatter.clear();
'''

## Notes

### Differences from other forks

* All classes available from 'libphonenumber' are exported as-is. No magic methods.
...
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.createFormattingTemplate_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>createFormattingTemplate_ (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.createFormattingTemplate_)
- description and source-code
```javascript
createFormattingTemplate_ = function (a) {
  var b = a.getPatternOrDefault();
  if (-1 != b.indexOf("|")) {
    return !1;
  }
  b = b.replace(i18n.phonenumbers.AsYouTypeFormatter.CHARACTER_CLASS_PATTERN_, "\\d");
  b = b.replace(i18n.phonenumbers.AsYouTypeFormatter.STANDALONE_DIGIT_PATTERN_, "\\d");
  this.formattingTemplate_.clear();
  a = this.getFormattingTemplate_(b, a.getFormatOrDefault());
  return 0 < a.length ? (this.formattingTemplate_.append(a), !0) : !1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.getAvailableFormats_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>getAvailableFormats_ (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.getAvailableFormats_)
- description and source-code
```javascript
getAvailableFormats_ = function (a) {
  for (var b = this.isCompleteNumber_ && 0 < this.currentMetadata_.intlNumberFormatCount() ? this.currentMetadata_.intlNumberFormatArray
() : this.currentMetadata_.numberFormatArray(), c = b.length, d = 0;d < c;++d) {
    var e = b[d];
    (!this.currentMetadata_.hasNationalPrefix() || this.isCompleteNumber_ || e.getNationalPrefixOptionalWhenFormatting() || this
.phoneUtil_.formattingRuleHasFirstGroupOnly(e.getNationalPrefixFormattingRuleOrDefault())) && this.isFormatEligible_(e.getFormatOrDefault
()) && this.possibleFormats_.push(e);
  }
  this.narrowDownPossibleFormats_(a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.getExtractedNationalPrefix_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>getExtractedNationalPrefix_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.getExtractedNationalPrefix_)
- description and source-code
```javascript
getExtractedNationalPrefix_ = function () {
  return this.extractedNationalPrefix_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.getFormattingTemplate_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>getFormattingTemplate_ (a, b)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.getFormattingTemplate_)
- description and source-code
```javascript
getFormattingTemplate_ = function (a, b) {
  var c = "999999999999999".match(a)[0];
  if (c.length < this.nationalNumber_.getLength()) {
    return "";
  }
  c = c.replace(new RegExp(a, "g"), b);
  return c = c.replace(RegExp("9", "g"), this.DIGIT_PLACEHOLDER_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.getMetadataForRegion_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>getMetadataForRegion_ (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.getMetadataForRegion_)
- description and source-code
```javascript
getMetadataForRegion_ = function (a) {
  a = this.phoneUtil_.getCountryCodeForRegion(a);
  a = this.phoneUtil_.getRegionCodeForCountryCode(a);
  a = this.phoneUtil_.getMetadataForRegion(a);
  return null != a ? a : i18n.phonenumbers.AsYouTypeFormatter.EMPTY_METADATA_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.getRememberedPosition"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>getRememberedPosition ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.getRememberedPosition)
- description and source-code
```javascript
getRememberedPosition = function () {
  if (!this.ableToFormat_) {
    return this.originalPosition_;
  }
  for (var a = 0, b = 0, c = this.accruedInputWithoutFormatting_.toString(), d = this.currentOutput_.toString();a < this.positionToRemember_
 && b < d.length;) {
    c.charAt(a) == d.charAt(b) && a++, b++;
  }
  return b;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.inputAccruedNationalNumber_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>inputAccruedNationalNumber_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.inputAccruedNationalNumber_)
- description and source-code
```javascript
inputAccruedNationalNumber_ = function () {
  var a = this.nationalNumber_.toString(), b = a.length;
  if (0 < b) {
    for (var c = "", d = 0;d < b;d++) {
      c = this.inputDigitHelper_(a.charAt(d));
    }
    return this.ableToFormat_ ? this.appendNationalNumber_(c) : this.accruedInput_.toString();
  }
  return this.prefixBeforeNationalNumber_.toString();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.inputDigit"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>inputDigit (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.inputDigit)
- description and source-code
```javascript
inputDigit = function (a) {
  return this.currentOutput_ = this.inputDigitWithOptionToRememberPosition_(a, !1);
}
```
- example usage
```shell
...
#### Using the "As You Type" Formatter

'''js
// Require 'AsYouTypeFormatter'.
var AsYouTypeFormatter = require('google-libphonenumber').AsYouTypeFormatter;
var formatter = new AsYouTypeFormatter('US');

console.log(formatter.inputDigit('6')); // => 6
console.log(formatter.inputDigit('5')); // => 65
console.log(formatter.inputDigit('0')); // => 650
console.log(formatter.inputDigit('2')); // => 650-2
console.log(formatter.inputDigit('5')); // => 650-25
console.log(formatter.inputDigit('3')); // => 650-253
console.log(formatter.inputDigit('2')); // => 650-2532
console.log(formatter.inputDigit('2')); // => (650) 253-22
...
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.inputDigitAndRememberPosition"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>inputDigitAndRememberPosition (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.inputDigitAndRememberPosition)
- description and source-code
```javascript
inputDigitAndRememberPosition = function (a) {
  return this.currentOutput_ = this.inputDigitWithOptionToRememberPosition_(a, !0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.inputDigitHelper_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>inputDigitHelper_ (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.inputDigitHelper_)
- description and source-code
```javascript
inputDigitHelper_ = function (a) {
  var b = this.formattingTemplate_.toString();
  if (0 <= b.substring(this.lastMatchPosition_).search(this.DIGIT_PATTERN_)) {
    var c = b.search(this.DIGIT_PATTERN_);
    a = b.replace(this.DIGIT_PATTERN_, a);
    this.formattingTemplate_.clear();
    this.formattingTemplate_.append(a);
    this.lastMatchPosition_ = c;
    return a.substring(0, this.lastMatchPosition_ + 1);
  }
  1 == this.possibleFormats_.length && (this.ableToFormat_ = !1);
  this.currentFormattingPattern_ = "";
  return this.accruedInput_.toString();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.inputDigitWithOptionToRememberPosition_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>inputDigitWithOptionToRememberPosition_ (a, b)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.inputDigitWithOptionToRememberPosition_)
- description and source-code
```javascript
inputDigitWithOptionToRememberPosition_ = function (a, b) {
  this.accruedInput_.append(a);
  b && (this.originalPosition_ = this.accruedInput_.getLength());
  this.isDigitOrLeadingPlusSign_(a) ? a = this.normalizeAndAccrueDigitsAndPlusSign_(a, b) : (this.ableToFormat_ = !1, this.inputHasFormatting_
 = !0);
  if (!this.ableToFormat_) {
    if (!this.inputHasFormatting_) {
      if (this.attemptToExtractIdd_()) {
        if (this.attemptToExtractCountryCallingCode_()) {
          return this.attemptToChoosePatternWithPrefixExtracted_();
        }
      } else {
        if (this.ableToExtractLongerNdd_()) {
          return this.prefixBeforeNationalNumber_.append(i18n.phonenumbers.AsYouTypeFormatter.SEPARATOR_BEFORE_NATIONAL_NUMBER_),
this.attemptToChoosePatternWithPrefixExtracted_();
        }
      }
    }
    return this.accruedInput_.toString();
  }
  switch(this.accruedInputWithoutFormatting_.getLength()) {
    case 0:
    case 1:
    case 2:
      return this.accruedInput_.toString();
    case 3:
      if (this.attemptToExtractIdd_()) {
        this.isExpectingCountryCallingCode_ = !0;
      } else {
        return this.extractedNationalPrefix_ = this.removeNationalPrefixFromNationalNumber_(), this.attemptToChooseFormattingPattern_
();
      }
    default:
      if (this.isExpectingCountryCallingCode_) {
        return this.attemptToExtractCountryCallingCode_() && (this.isExpectingCountryCallingCode_ = !1), this.prefixBeforeNationalNumber_
.toString() + this.nationalNumber_.toString();
      }
      if (0 < this.possibleFormats_.length) {
        var c = this.inputDigitHelper_(a), d = this.attemptToFormatAccruedDigits_();
        if (0 < d.length) {
          return d;
        }
        this.narrowDownPossibleFormats_(this.nationalNumber_.toString());
        return this.maybeCreateNewTemplate_() ? this.inputAccruedNationalNumber_() : this.ableToFormat_ ? this.appendNationalNumber_
(c) : this.accruedInput_.toString();
      }
      return this.attemptToChooseFormattingPattern_();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.isDigitOrLeadingPlusSign_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>isDigitOrLeadingPlusSign_ (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.isDigitOrLeadingPlusSign_)
- description and source-code
```javascript
isDigitOrLeadingPlusSign_ = function (a) {
  return i18n.phonenumbers.PhoneNumberUtil.CAPTURING_DIGIT_PATTERN.test(a) || 1 == this.accruedInput_.getLength() && i18n.phonenumbers
.PhoneNumberUtil.PLUS_CHARS_PATTERN.test(a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.isFormatEligible_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>isFormatEligible_ (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.isFormatEligible_)
- description and source-code
```javascript
isFormatEligible_ = function (a) {
  return i18n.phonenumbers.AsYouTypeFormatter.ELIGIBLE_FORMAT_PATTERN_.test(a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.isNanpaNumberWithNationalPrefix_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>isNanpaNumberWithNationalPrefix_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.isNanpaNumberWithNationalPrefix_)
- description and source-code
```javascript
isNanpaNumberWithNationalPrefix_ = function () {
  if (1 != this.currentMetadata_.getCountryCode()) {
    return !1;
  }
  var a = this.nationalNumber_.toString();
  return "1" == a.charAt(0) && "0" != a.charAt(1) && "1" != a.charAt(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.maybeCreateNewTemplate_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>maybeCreateNewTemplate_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.maybeCreateNewTemplate_)
- description and source-code
```javascript
maybeCreateNewTemplate_ = function () {
  for (var a = this.possibleFormats_.length, b = 0;b < a;++b) {
    var c = this.possibleFormats_[b], d = c.getPatternOrDefault();
    if (this.currentFormattingPattern_ == d) {
      return !1;
    }
    if (this.createFormattingTemplate_(c)) {
      return this.currentFormattingPattern_ = d, this.shouldAddSpaceAfterNationalPrefix_ = i18n.phonenumbers.AsYouTypeFormatter.
NATIONAL_PREFIX_SEPARATORS_PATTERN_.test(c.getNationalPrefixFormattingRule()), this.lastMatchPosition_ = 0, !0;
    }
  }
  return this.ableToFormat_ = !1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.narrowDownPossibleFormats_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>narrowDownPossibleFormats_ (a)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.narrowDownPossibleFormats_)
- description and source-code
```javascript
narrowDownPossibleFormats_ = function (a) {
  for (var b = [], c = a.length - i18n.phonenumbers.AsYouTypeFormatter.MIN_LEADING_DIGITS_LENGTH_, d = this.possibleFormats_.length
, e = 0;e < d;++e) {
    var f = this.possibleFormats_[e];
    if (0 == f.leadingDigitsPatternCount()) {
      b.push(this.possibleFormats_[e]);
    } else {
      var g = Math.min(c, f.leadingDigitsPatternCount() - 1), f = f.getLeadingDigitsPattern(g);
      0 == a.search(f) && b.push(this.possibleFormats_[e]);
    }
  }
  this.possibleFormats_ = b;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.normalizeAndAccrueDigitsAndPlusSign_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>normalizeAndAccrueDigitsAndPlusSign_ (a, b)](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.normalizeAndAccrueDigitsAndPlusSign_)
- description and source-code
```javascript
normalizeAndAccrueDigitsAndPlusSign_ = function (a, b) {
  var c;
  a == i18n.phonenumbers.PhoneNumberUtil.PLUS_SIGN ? (c = a, this.accruedInputWithoutFormatting_.append(a)) : (c = i18n.phonenumbers
.PhoneNumberUtil.DIGIT_MAPPINGS[a], this.accruedInputWithoutFormatting_.append(c), this.nationalNumber_.append(c));
  b && (this.positionToRemember_ = this.accruedInputWithoutFormatting_.getLength());
  return c;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.removeNationalPrefixFromNationalNumber_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.AsYouTypeFormatter.prototype.</span>removeNationalPrefixFromNationalNumber_ ()](#apidoc.element.google-libphonenumber.AsYouTypeFormatter.prototype.removeNationalPrefixFromNationalNumber_)
- description and source-code
```javascript
removeNationalPrefixFromNationalNumber_ = function () {
  var a = this.nationalNumber_.toString(), b = 0;
  if (this.isNanpaNumberWithNationalPrefix_()) {
    b = 1, this.prefixBeforeNationalNumber_.append("1").append(i18n.phonenumbers.AsYouTypeFormatter.SEPARATOR_BEFORE_NATIONAL_NUMBER_
), this.isCompleteNumber_ = !0;
  } else {
    if (this.currentMetadata_.hasNationalPrefixForParsing()) {
      var c = new RegExp("^(?:" + this.currentMetadata_.getNationalPrefixForParsing() + ")"), c = a.match(c);
      null != c && null != c[0] && 0 < c[0].length && (this.isCompleteNumber_ = !0, b = c[0].length, this.prefixBeforeNationalNumber_
.append(a.substring(0, b)));
    }
  }
  this.nationalNumber_.clear();
  this.nationalNumber_.append(a.substring(b));
  return a.substring(0, b);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.google-libphonenumber.NumberFormat"></a>[module google-libphonenumber.NumberFormat](#apidoc.module.google-libphonenumber.NumberFormat)

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.NumberFormat"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.</span>NumberFormat ()](#apidoc.element.google-libphonenumber.NumberFormat.NumberFormat)
- description and source-code
```javascript
NumberFormat = function () {
  goog.proto2.Message.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.base"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.</span>base (a, c, f)](#apidoc.element.google-libphonenumber.NumberFormat.base)
- description and source-code
```javascript
base = function (a, c, f) {
  for (var d = Array(arguments.length - 2), e = 2;e < arguments.length;e++) {
    d[e - 2] = arguments[e];
  }
  return b.prototype[c].apply(a, d);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.getDescriptor"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.NumberFormat.getDescriptor)
- description and source-code
```javascript
getDescriptor = function () {
  var a = i18n.phonenumbers.NumberFormat.descriptor_;
  a || (i18n.phonenumbers.NumberFormat.descriptor_ = a = goog.proto2.Message.createDescriptor(i18n.phonenumbers.NumberFormat, {0
:{name:"NumberFormat", fullName:"i18n.phonenumbers.NumberFormat"}, 1:{name:"pattern", required:!0, fieldType:goog.proto2.Message
.FieldType.STRING, type:String}, 2:{name:"format", required:!0, fieldType:goog.proto2.Message.FieldType.STRING, type:String}, 3:{
name:"leading_digits_pattern", repeated:!0, fieldType:goog.proto2.Message.FieldType.STRING, type:String}, 4:{name:"national_prefix_formatting_rule
",
  fieldType:goog.proto2.Message.FieldType.STRING, type:String}, 6:{name:"national_prefix_optional_when_formatting", fieldType:goog
.proto2.Message.FieldType.BOOL, type:Boolean}, 5:{name:"domestic_carrier_code_formatting_rule", fieldType:goog.proto2.Message.FieldType
.STRING, type:String}}));
  return a;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.google-libphonenumber.NumberFormat.prototype"></a>[module google-libphonenumber.NumberFormat.prototype](#apidoc.module.google-libphonenumber.NumberFormat.prototype)

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.addLeadingDigitsPattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>addLeadingDigitsPattern (a)](#apidoc.element.google-libphonenumber.NumberFormat.prototype.addLeadingDigitsPattern)
- description and source-code
```javascript
addLeadingDigitsPattern = function (a) {
  this.add$Value(3, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.clearDomesticCarrierCodeFormattingRule"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>clearDomesticCarrierCodeFormattingRule ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.clearDomesticCarrierCodeFormattingRule)
- description and source-code
```javascript
clearDomesticCarrierCodeFormattingRule = function () {
  this.clear$Field(5);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.clearFormat"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>clearFormat ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.clearFormat)
- description and source-code
```javascript
clearFormat = function () {
  this.clear$Field(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.clearLeadingDigitsPattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>clearLeadingDigitsPattern ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.clearLeadingDigitsPattern)
- description and source-code
```javascript
clearLeadingDigitsPattern = function () {
  this.clear$Field(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.clearNationalPrefixFormattingRule"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>clearNationalPrefixFormattingRule ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.clearNationalPrefixFormattingRule)
- description and source-code
```javascript
clearNationalPrefixFormattingRule = function () {
  this.clear$Field(4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.clearNationalPrefixOptionalWhenFormatting"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>clearNationalPrefixOptionalWhenFormatting ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.clearNationalPrefixOptionalWhenFormatting)
- description and source-code
```javascript
clearNationalPrefixOptionalWhenFormatting = function () {
  this.clear$Field(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.clearPattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>clearPattern ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.clearPattern)
- description and source-code
```javascript
clearPattern = function () {
  this.clear$Field(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.constructor"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>constructor ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  goog.proto2.Message.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.domesticCarrierCodeFormattingRuleCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>domesticCarrierCodeFormattingRuleCount ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.domesticCarrierCodeFormattingRuleCount)
- description and source-code
```javascript
domesticCarrierCodeFormattingRuleCount = function () {
  return this.count$Values(5);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.formatCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>formatCount ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.formatCount)
- description and source-code
```javascript
formatCount = function () {
  return this.count$Values(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.getDescriptor"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getDescriptor)
- description and source-code
```javascript
getDescriptor = function () {
  var a = i18n.phonenumbers.NumberFormat.descriptor_;
  a || (i18n.phonenumbers.NumberFormat.descriptor_ = a = goog.proto2.Message.createDescriptor(i18n.phonenumbers.NumberFormat, {0
:{name:"NumberFormat", fullName:"i18n.phonenumbers.NumberFormat"}, 1:{name:"pattern", required:!0, fieldType:goog.proto2.Message
.FieldType.STRING, type:String}, 2:{name:"format", required:!0, fieldType:goog.proto2.Message.FieldType.STRING, type:String}, 3:{
name:"leading_digits_pattern", repeated:!0, fieldType:goog.proto2.Message.FieldType.STRING, type:String}, 4:{name:"national_prefix_formatting_rule
",
  fieldType:goog.proto2.Message.FieldType.STRING, type:String}, 6:{name:"national_prefix_optional_when_formatting", fieldType:goog
.proto2.Message.FieldType.BOOL, type:Boolean}, 5:{name:"domestic_carrier_code_formatting_rule", fieldType:goog.proto2.Message.FieldType
.STRING, type:String}}));
  return a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.getDomesticCarrierCodeFormattingRule"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getDomesticCarrierCodeFormattingRule ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getDomesticCarrierCodeFormattingRule)
- description and source-code
```javascript
getDomesticCarrierCodeFormattingRule = function () {
  return this.get$Value(5);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.getDomesticCarrierCodeFormattingRuleOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getDomesticCarrierCodeFormattingRuleOrDefault ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getDomesticCarrierCodeFormattingRuleOrDefault)
- description and source-code
```javascript
getDomesticCarrierCodeFormattingRuleOrDefault = function () {
  return this.get$ValueOrDefault(5);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.getFormat"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getFormat ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getFormat)
- description and source-code
```javascript
getFormat = function () {
  return this.get$Value(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.getFormatOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getFormatOrDefault ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getFormatOrDefault)
- description and source-code
```javascript
getFormatOrDefault = function () {
  return this.get$ValueOrDefault(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.getLeadingDigitsPattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getLeadingDigitsPattern (a)](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getLeadingDigitsPattern)
- description and source-code
```javascript
getLeadingDigitsPattern = function (a) {
  return this.get$Value(3, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.getLeadingDigitsPatternOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getLeadingDigitsPatternOrDefault (a)](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getLeadingDigitsPatternOrDefault)
- description and source-code
```javascript
getLeadingDigitsPatternOrDefault = function (a) {
  return this.get$ValueOrDefault(3, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.getNationalPrefixFormattingRule"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getNationalPrefixFormattingRule ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getNationalPrefixFormattingRule)
- description and source-code
```javascript
getNationalPrefixFormattingRule = function () {
  return this.get$Value(4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.getNationalPrefixFormattingRuleOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getNationalPrefixFormattingRuleOrDefault ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getNationalPrefixFormattingRuleOrDefault)
- description and source-code
```javascript
getNationalPrefixFormattingRuleOrDefault = function () {
  return this.get$ValueOrDefault(4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.getNationalPrefixOptionalWhenFormatting"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getNationalPrefixOptionalWhenFormatting ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getNationalPrefixOptionalWhenFormatting)
- description and source-code
```javascript
getNationalPrefixOptionalWhenFormatting = function () {
  return this.get$Value(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.getNationalPrefixOptionalWhenFormattingOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getNationalPrefixOptionalWhenFormattingOrDefault ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getNationalPrefixOptionalWhenFormattingOrDefault)
- description and source-code
```javascript
getNationalPrefixOptionalWhenFormattingOrDefault = function () {
  return this.get$ValueOrDefault(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.getPattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getPattern ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getPattern)
- description and source-code
```javascript
getPattern = function () {
  return this.get$Value(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.getPatternOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>getPatternOrDefault ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.getPatternOrDefault)
- description and source-code
```javascript
getPatternOrDefault = function () {
  return this.get$ValueOrDefault(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.hasDomesticCarrierCodeFormattingRule"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>hasDomesticCarrierCodeFormattingRule ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.hasDomesticCarrierCodeFormattingRule)
- description and source-code
```javascript
hasDomesticCarrierCodeFormattingRule = function () {
  return this.has$Value(5);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.hasFormat"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>hasFormat ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.hasFormat)
- description and source-code
```javascript
hasFormat = function () {
  return this.has$Value(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.hasLeadingDigitsPattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>hasLeadingDigitsPattern ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.hasLeadingDigitsPattern)
- description and source-code
```javascript
hasLeadingDigitsPattern = function () {
  return this.has$Value(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.hasNationalPrefixFormattingRule"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>hasNationalPrefixFormattingRule ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.hasNationalPrefixFormattingRule)
- description and source-code
```javascript
hasNationalPrefixFormattingRule = function () {
  return this.has$Value(4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.hasNationalPrefixOptionalWhenFormatting"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>hasNationalPrefixOptionalWhenFormatting ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.hasNationalPrefixOptionalWhenFormatting)
- description and source-code
```javascript
hasNationalPrefixOptionalWhenFormatting = function () {
  return this.has$Value(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.hasPattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>hasPattern ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.hasPattern)
- description and source-code
```javascript
hasPattern = function () {
  return this.has$Value(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.leadingDigitsPatternArray"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>leadingDigitsPatternArray ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.leadingDigitsPatternArray)
- description and source-code
```javascript
leadingDigitsPatternArray = function () {
  return this.array$Values(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.leadingDigitsPatternCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>leadingDigitsPatternCount ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.leadingDigitsPatternCount)
- description and source-code
```javascript
leadingDigitsPatternCount = function () {
  return this.count$Values(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.nationalPrefixFormattingRuleCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>nationalPrefixFormattingRuleCount ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.nationalPrefixFormattingRuleCount)
- description and source-code
```javascript
nationalPrefixFormattingRuleCount = function () {
  return this.count$Values(4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.nationalPrefixOptionalWhenFormattingCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>nationalPrefixOptionalWhenFormattingCount ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.nationalPrefixOptionalWhenFormattingCount)
- description and source-code
```javascript
nationalPrefixOptionalWhenFormattingCount = function () {
  return this.count$Values(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.patternCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>patternCount ()](#apidoc.element.google-libphonenumber.NumberFormat.prototype.patternCount)
- description and source-code
```javascript
patternCount = function () {
  return this.count$Values(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.setDomesticCarrierCodeFormattingRule"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>setDomesticCarrierCodeFormattingRule (a)](#apidoc.element.google-libphonenumber.NumberFormat.prototype.setDomesticCarrierCodeFormattingRule)
- description and source-code
```javascript
setDomesticCarrierCodeFormattingRule = function (a) {
  this.set$Value(5, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.setFormat"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>setFormat (a)](#apidoc.element.google-libphonenumber.NumberFormat.prototype.setFormat)
- description and source-code
```javascript
setFormat = function (a) {
  this.set$Value(2, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.setNationalPrefixFormattingRule"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>setNationalPrefixFormattingRule (a)](#apidoc.element.google-libphonenumber.NumberFormat.prototype.setNationalPrefixFormattingRule)
- description and source-code
```javascript
setNationalPrefixFormattingRule = function (a) {
  this.set$Value(4, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.setNationalPrefixOptionalWhenFormatting"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>setNationalPrefixOptionalWhenFormatting (a)](#apidoc.element.google-libphonenumber.NumberFormat.prototype.setNationalPrefixOptionalWhenFormatting)
- description and source-code
```javascript
setNationalPrefixOptionalWhenFormatting = function (a) {
  this.set$Value(6, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.prototype.setPattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.prototype.</span>setPattern (a)](#apidoc.element.google-libphonenumber.NumberFormat.prototype.setPattern)
- description and source-code
```javascript
setPattern = function (a) {
  this.set$Value(1, a);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.google-libphonenumber.NumberFormat.superClass_"></a>[module google-libphonenumber.NumberFormat.superClass_](#apidoc.module.google-libphonenumber.NumberFormat.superClass_)

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.add"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>add (a, b)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.add)
- description and source-code
```javascript
add = function (a, b) {
  goog.asserts.assert(a.getContainingType() == this.getDescriptor(), "The current message does not contain the given field");
  this.add$Value(a.getTag(), b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.arrayOf"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>arrayOf (a)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.arrayOf)
- description and source-code
```javascript
arrayOf = function (a) {
  goog.asserts.assert(a.getContainingType() == this.getDescriptor(), "The current message does not contain the given field");
  return this.array$Values(a.getTag());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.checkFieldType_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>checkFieldType_ (a, b)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.checkFieldType_)
- description and source-code
```javascript
checkFieldType_ = function (a, b) {
  a.getFieldType() == goog.proto2.FieldDescriptor.FieldType.ENUM ? goog.asserts.assertNumber(b) : goog.asserts.assert(Object(b).
constructor == a.getNativeType());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.clear"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>clear (a)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.clear)
- description and source-code
```javascript
clear = function (a) {
  goog.asserts.assert(a.getContainingType() == this.getDescriptor(), "The current message does not contain the given field");
  this.clear$Field(a.getTag());
}
```
- example usage
```shell
...
console.log(formatter.inputDigit('0')); // => 650
console.log(formatter.inputDigit('2')); // => 650-2
console.log(formatter.inputDigit('5')); // => 650-25
console.log(formatter.inputDigit('3')); // => 650-253
console.log(formatter.inputDigit('2')); // => 650-2532
console.log(formatter.inputDigit('2')); // => (650) 253-22

formatter.clear();
'''

## Notes

### Differences from other forks

* All classes available from 'libphonenumber' are exported as-is. No magic methods.
...
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.clone"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>clone ()](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.clone)
- description and source-code
```javascript
clone = function () {
  var a = new this.constructor;
  a.copyFrom(this);
  return a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.copyFrom"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>copyFrom (a)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.copyFrom)
- description and source-code
```javascript
copyFrom = function (a) {
  goog.asserts.assert(this.constructor == a.constructor, "The source message must have the same type.");
  this != a && (this.values_ = {}, this.deserializedFields_ && (this.deserializedFields_ = {}), this.mergeFrom(a));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.countOf"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>countOf (a)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.countOf)
- description and source-code
```javascript
countOf = function (a) {
  goog.asserts.assert(a.getContainingType() == this.getDescriptor(), "The current message does not contain the given field");
  return this.count$Values(a.getTag());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.equals"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>equals (a)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.equals)
- description and source-code
```javascript
equals = function (a) {
  if (!a || this.constructor != a.constructor) {
    return !1;
  }
  for (var b = this.getDescriptor().getFields(), c = 0;c < b.length;c++) {
    var d = b[c], e = d.getTag();
    if (this.has$Value(e) != a.has$Value(e)) {
      return !1;
    }
    if (this.has$Value(e)) {
      var f = d.isCompositeType(), g = this.getValueForTag_(e), e = a.getValueForTag_(e);
      if (d.isRepeated()) {
        if (g.length != e.length) {
          return !1;
        }
        for (d = 0;d < g.length;d++) {
          var h = g[d], k = e[d];
          if (f ? !h.equals(k) : h != k) {
            return !1;
          }
        }
      } else {
        if (f ? !g.equals(e) : g != e) {
          return !1;
        }
      }
    }
  }
  return !0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.forEachUnknown"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>forEachUnknown (a, b)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.forEachUnknown)
- description and source-code
```javascript
forEachUnknown = function (a, b) {
  var c = b || this, d;
  for (d in this.values_) {
    var e = Number(d);
    this.fields_[e] || a.call(c, e, this.values_[d]);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.get"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>get (a, b)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.get)
- description and source-code
```javascript
get = function (a, b) {
  goog.asserts.assert(a.getContainingType() == this.getDescriptor(), "The current message does not contain the given field");
  return this.get$Value(a.getTag(), b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.getDescriptor"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.getDescriptor)
- description and source-code
```javascript
getDescriptor = function () {
  throw Error("unimplemented abstract method");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.getOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>getOrDefault (a, b)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.getOrDefault)
- description and source-code
```javascript
getOrDefault = function (a, b) {
  goog.asserts.assert(a.getContainingType() == this.getDescriptor(), "The current message does not contain the given field");
  return this.get$ValueOrDefault(a.getTag(), b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.getValueForTag_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>getValueForTag_ (a)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.getValueForTag_)
- description and source-code
```javascript
getValueForTag_ = function (a) {
  var b = this.values_[a];
  return goog.isDefAndNotNull(b) ? this.lazyDeserializer_ ? a in this.deserializedFields_ ? this.deserializedFields_[a] : (b = this
.lazyDeserializer_.deserializeField(this, this.fields_[a], b), this.deserializedFields_[a] = b) : b : null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.has"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>has (a)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.has)
- description and source-code
```javascript
has = function (a) {
  goog.asserts.assert(a.getContainingType() == this.getDescriptor(), "The current message does not contain the given field");
  return this.has$Value(a.getTag());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.initDefaults"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>initDefaults (a)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.initDefaults)
- description and source-code
```javascript
initDefaults = function (a) {
  for (var b = this.getDescriptor().getFields(), c = 0;c < b.length;c++) {
    var d = b[c], e = d.getTag(), f = d.isCompositeType();
    this.has$Value(e) || d.isRepeated() || (f ? this.values_[e] = new (d.getNativeType()) : a && (this.values_[e] = d.getDefaultValue
()));
    if (f) {
      if (d.isRepeated()) {
        for (d = this.array$Values(e), e = 0;e < d.length;e++) {
          d[e].initDefaults(a);
        }
      } else {
        this.get$Value(e).initDefaults(a);
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.initializeForLazyDeserializer"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>initializeForLazyDeserializer (a, b)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.initializeForLazyDeserializer)
- description and source-code
```javascript
initializeForLazyDeserializer = function (a, b) {
  this.lazyDeserializer_ = a;
  this.values_ = b;
  this.deserializedFields_ = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.mergeFrom"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>mergeFrom (a)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.mergeFrom)
- description and source-code
```javascript
mergeFrom = function (a) {
  goog.asserts.assert(this.constructor == a.constructor, "The source message must have the same type.");
  for (var b = this.getDescriptor().getFields(), c = 0;c < b.length;c++) {
    var d = b[c], e = d.getTag();
    if (a.has$Value(e)) {
      this.deserializedFields_ && delete this.deserializedFields_[d.getTag()];
      var f = d.isCompositeType();
      if (d.isRepeated()) {
        for (var d = a.array$Values(e), g = 0;g < d.length;g++) {
          this.add$Value(e, f ? d[g].clone() : d[g]);
        }
      } else {
        d = a.getValueForTag_(e), f ? (f = this.getValueForTag_(e)) ? f.mergeFrom(d) : this.set$Value(e, d.clone()) : this.set$Value
(e, d);
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.set"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>set (a, b)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.set)
- description and source-code
```javascript
set = function (a, b) {
  goog.asserts.assert(a.getContainingType() == this.getDescriptor(), "The current message does not contain the given field");
  this.set$Value(a.getTag(), b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.NumberFormat.superClass_.setUnknown"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.NumberFormat.superClass_.</span>setUnknown (a, b)](#apidoc.element.google-libphonenumber.NumberFormat.superClass_.setUnknown)
- description and source-code
```javascript
setUnknown = function (a, b) {
  goog.asserts.assert(!this.fields_[a], "Field is not unknown in this message");
  goog.asserts.assert(1 <= a, "Tag " + a + ' has value "' + b + '" in descriptor ' + this.getDescriptor().getName());
  goog.asserts.assert(null !== b, "Value cannot be null");
  this.values_[a] = b;
  this.deserializedFields_ && delete this.deserializedFields_[a];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.google-libphonenumber.PhoneMetadata"></a>[module google-libphonenumber.PhoneMetadata](#apidoc.module.google-libphonenumber.PhoneMetadata)

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.PhoneMetadata"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneMetadata ()](#apidoc.element.google-libphonenumber.PhoneMetadata.PhoneMetadata)
- description and source-code
```javascript
PhoneMetadata = function () {
  goog.proto2.Message.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.base"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.</span>base (a, c, f)](#apidoc.element.google-libphonenumber.PhoneMetadata.base)
- description and source-code
```javascript
base = function (a, c, f) {
  for (var d = Array(arguments.length - 2), e = 2;e < arguments.length;e++) {
    d[e - 2] = arguments[e];
  }
  return b.prototype[c].apply(a, d);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.getDescriptor"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.PhoneMetadata.getDescriptor)
- description and source-code
```javascript
getDescriptor = function () {
  var a = i18n.phonenumbers.PhoneMetadata.descriptor_;
  a || (i18n.phonenumbers.PhoneMetadata.descriptor_ = a = goog.proto2.Message.createDescriptor(i18n.phonenumbers.PhoneMetadata, {
0:{name:"PhoneMetadata", fullName:"i18n.phonenumbers.PhoneMetadata"}, 1:{name:"general_desc", fieldType:goog.proto2.Message.FieldType
.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc}, 2:{name:"fixed_line", fieldType:goog.proto2.Message.FieldType.MESSAGE, type:i18n
.phonenumbers.PhoneNumberDesc}, 3:{name:"mobile", fieldType:goog.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc
},
  4:{name:"toll_free", fieldType:goog.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc}, 5:{name:"premium_rate
", fieldType:goog.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc}, 6:{name:"shared_cost", fieldType:goog
.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc}, 7:{name:"personal_number", fieldType:goog.proto2.Message
.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc}, 8:{name:"voip", fieldType:goog.proto2.Message.FieldType.MESSAGE,
  type:i18n.phonenumbers.PhoneNumberDesc}, 21:{name:"pager", fieldType:goog.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers
.PhoneNumberDesc}, 25:{name:"uan", fieldType:goog.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc}, 27:{
name:"emergency", fieldType:goog.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc}, 28:{name:"voicemail",
fieldType:goog.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc}, 24:{name:"no_international_dialling",
  fieldType:goog.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc}, 9:{name:"id", required:!0, fieldType
:goog.proto2.Message.FieldType.STRING, type:String}, 10:{name:"country_code", fieldType:goog.proto2.Message.FieldType.INT32, type
:Number}, 11:{name:"international_prefix", fieldType:goog.proto2.Message.FieldType.STRING, type:String}, 17:{name:"preferred_international_prefix
", fieldType:goog.proto2.Message.FieldType.STRING, type:String}, 12:{name:"national_prefix", fieldType:goog.proto2.Message.FieldType
.STRING,
  type:String}, 13:{name:"preferred_extn_prefix", fieldType:goog.proto2.Message.FieldType.STRING, type:String}, 15:{name:"national_prefix_for_parsing
", fieldType:goog.proto2.Message.FieldType.STRING, type:String}, 16:{name:"national_prefix_transform_rule", fieldType:goog.proto2
.Message.FieldType.STRING, type:String}, 18:{name:"same_mobile_and_fixed_line_pattern", fieldType:goog.proto2.Message.FieldType.
BOOL, defaultValue:!1, type:Boolean}, 19:{name:"number_format", repeated:!0, fieldType:goog.proto2.Message.FieldType.MESSAGE,
  type:i18n.phonenumbers.NumberFormat}, 20:{name:"intl_number_format", repeated:!0, fieldType:goog.proto2.Message.FieldType.MESSAGE
, type:i18n.phonenumbers.NumberFormat}, 22:{name:"main_country_for_code", fieldType:goog.proto2.Message.FieldType.BOOL, defaultValue
:!1, type:Boolean}, 23:{name:"leading_digits", fieldType:goog.proto2.Message.FieldType.STRING, type:String}, 26:{name:"leading_zero_possible
", fieldType:goog.proto2.Message.FieldType.BOOL, defaultValue:!1, type:Boolean}}));
  return a;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.google-libphonenumber.PhoneMetadata.descriptor_"></a>[module google-libphonenumber.PhoneMetadata.descriptor_](#apidoc.module.google-libphonenumber.PhoneMetadata.descriptor_)

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.descriptor_.messageType_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.descriptor_.</span>messageType_ ()](#apidoc.element.google-libphonenumber.PhoneMetadata.descriptor_.messageType_)
- description and source-code
```javascript
messageType_ = function () {
  goog.proto2.Message.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.google-libphonenumber.PhoneMetadata.prototype"></a>[module google-libphonenumber.PhoneMetadata.prototype](#apidoc.module.google-libphonenumber.PhoneMetadata.prototype)

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.addIntlNumberFormat"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>addIntlNumberFormat (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.addIntlNumberFormat)
- description and source-code
```javascript
addIntlNumberFormat = function (a) {
  this.add$Value(20, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.addNumberFormat"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>addNumberFormat (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.addNumberFormat)
- description and source-code
```javascript
addNumberFormat = function (a) {
  this.add$Value(19, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearCountryCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearCountryCode ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearCountryCode)
- description and source-code
```javascript
clearCountryCode = function () {
  this.clear$Field(10);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearEmergency"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearEmergency ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearEmergency)
- description and source-code
```javascript
clearEmergency = function () {
  this.clear$Field(27);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearFixedLine"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearFixedLine ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearFixedLine)
- description and source-code
```javascript
clearFixedLine = function () {
  this.clear$Field(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearGeneralDesc"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearGeneralDesc ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearGeneralDesc)
- description and source-code
```javascript
clearGeneralDesc = function () {
  this.clear$Field(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearId"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearId ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearId)
- description and source-code
```javascript
clearId = function () {
  this.clear$Field(9);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearInternationalPrefix"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearInternationalPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearInternationalPrefix)
- description and source-code
```javascript
clearInternationalPrefix = function () {
  this.clear$Field(11);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearIntlNumberFormat"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearIntlNumberFormat ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearIntlNumberFormat)
- description and source-code
```javascript
clearIntlNumberFormat = function () {
  this.clear$Field(20);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearLeadingDigits"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearLeadingDigits ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearLeadingDigits)
- description and source-code
```javascript
clearLeadingDigits = function () {
  this.clear$Field(23);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearLeadingZeroPossible"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearLeadingZeroPossible ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearLeadingZeroPossible)
- description and source-code
```javascript
clearLeadingZeroPossible = function () {
  this.clear$Field(26);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearMainCountryForCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearMainCountryForCode ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearMainCountryForCode)
- description and source-code
```javascript
clearMainCountryForCode = function () {
  this.clear$Field(22);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearMobile"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearMobile ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearMobile)
- description and source-code
```javascript
clearMobile = function () {
  this.clear$Field(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearNationalPrefix"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearNationalPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearNationalPrefix)
- description and source-code
```javascript
clearNationalPrefix = function () {
  this.clear$Field(12);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearNationalPrefixForParsing"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearNationalPrefixForParsing ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearNationalPrefixForParsing)
- description and source-code
```javascript
clearNationalPrefixForParsing = function () {
  this.clear$Field(15);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearNationalPrefixTransformRule"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearNationalPrefixTransformRule ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearNationalPrefixTransformRule)
- description and source-code
```javascript
clearNationalPrefixTransformRule = function () {
  this.clear$Field(16);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearNoInternationalDialling"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearNoInternationalDialling ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearNoInternationalDialling)
- description and source-code
```javascript
clearNoInternationalDialling = function () {
  this.clear$Field(24);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearNumberFormat"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearNumberFormat ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearNumberFormat)
- description and source-code
```javascript
clearNumberFormat = function () {
  this.clear$Field(19);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearPager"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearPager ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearPager)
- description and source-code
```javascript
clearPager = function () {
  this.clear$Field(21);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearPersonalNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearPersonalNumber ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearPersonalNumber)
- description and source-code
```javascript
clearPersonalNumber = function () {
  this.clear$Field(7);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearPreferredExtnPrefix"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearPreferredExtnPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearPreferredExtnPrefix)
- description and source-code
```javascript
clearPreferredExtnPrefix = function () {
  this.clear$Field(13);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearPreferredInternationalPrefix"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearPreferredInternationalPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearPreferredInternationalPrefix)
- description and source-code
```javascript
clearPreferredInternationalPrefix = function () {
  this.clear$Field(17);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearPremiumRate"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearPremiumRate ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearPremiumRate)
- description and source-code
```javascript
clearPremiumRate = function () {
  this.clear$Field(5);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearSameMobileAndFixedLinePattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearSameMobileAndFixedLinePattern ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearSameMobileAndFixedLinePattern)
- description and source-code
```javascript
clearSameMobileAndFixedLinePattern = function () {
  this.clear$Field(18);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearSharedCost"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearSharedCost ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearSharedCost)
- description and source-code
```javascript
clearSharedCost = function () {
  this.clear$Field(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearTollFree"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearTollFree ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearTollFree)
- description and source-code
```javascript
clearTollFree = function () {
  this.clear$Field(4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearUan"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearUan ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearUan)
- description and source-code
```javascript
clearUan = function () {
  this.clear$Field(25);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearVoicemail"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearVoicemail ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearVoicemail)
- description and source-code
```javascript
clearVoicemail = function () {
  this.clear$Field(28);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearVoip"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>clearVoip ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.clearVoip)
- description and source-code
```javascript
clearVoip = function () {
  this.clear$Field(8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.constructor"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>constructor ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  goog.proto2.Message.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.countryCodeCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>countryCodeCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.countryCodeCount)
- description and source-code
```javascript
countryCodeCount = function () {
  return this.count$Values(10);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.emergencyCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>emergencyCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.emergencyCount)
- description and source-code
```javascript
emergencyCount = function () {
  return this.count$Values(27);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.fixedLineCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>fixedLineCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.fixedLineCount)
- description and source-code
```javascript
fixedLineCount = function () {
  return this.count$Values(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.generalDescCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>generalDescCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.generalDescCount)
- description and source-code
```javascript
generalDescCount = function () {
  return this.count$Values(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getCountryCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getCountryCode ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getCountryCode)
- description and source-code
```javascript
getCountryCode = function () {
  return this.get$Value(10);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getCountryCodeOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getCountryCodeOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getCountryCodeOrDefault)
- description and source-code
```javascript
getCountryCodeOrDefault = function () {
  return this.get$ValueOrDefault(10);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getDescriptor"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getDescriptor)
- description and source-code
```javascript
getDescriptor = function () {
  var a = i18n.phonenumbers.PhoneMetadata.descriptor_;
  a || (i18n.phonenumbers.PhoneMetadata.descriptor_ = a = goog.proto2.Message.createDescriptor(i18n.phonenumbers.PhoneMetadata, {
0:{name:"PhoneMetadata", fullName:"i18n.phonenumbers.PhoneMetadata"}, 1:{name:"general_desc", fieldType:goog.proto2.Message.FieldType
.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc}, 2:{name:"fixed_line", fieldType:goog.proto2.Message.FieldType.MESSAGE, type:i18n
.phonenumbers.PhoneNumberDesc}, 3:{name:"mobile", fieldType:goog.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc
},
  4:{name:"toll_free", fieldType:goog.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc}, 5:{name:"premium_rate
", fieldType:goog.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc}, 6:{name:"shared_cost", fieldType:goog
.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc}, 7:{name:"personal_number", fieldType:goog.proto2.Message
.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc}, 8:{name:"voip", fieldType:goog.proto2.Message.FieldType.MESSAGE,
  type:i18n.phonenumbers.PhoneNumberDesc}, 21:{name:"pager", fieldType:goog.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers
.PhoneNumberDesc}, 25:{name:"uan", fieldType:goog.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc}, 27:{
name:"emergency", fieldType:goog.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc}, 28:{name:"voicemail",
fieldType:goog.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc}, 24:{name:"no_international_dialling",
  fieldType:goog.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneNumberDesc}, 9:{name:"id", required:!0, fieldType
:goog.proto2.Message.FieldType.STRING, type:String}, 10:{name:"country_code", fieldType:goog.proto2.Message.FieldType.INT32, type
:Number}, 11:{name:"international_prefix", fieldType:goog.proto2.Message.FieldType.STRING, type:String}, 17:{name:"preferred_international_prefix
", fieldType:goog.proto2.Message.FieldType.STRING, type:String}, 12:{name:"national_prefix", fieldType:goog.proto2.Message.FieldType
.STRING,
  type:String}, 13:{name:"preferred_extn_prefix", fieldType:goog.proto2.Message.FieldType.STRING, type:String}, 15:{name:"national_prefix_for_parsing
", fieldType:goog.proto2.Message.FieldType.STRING, type:String}, 16:{name:"national_prefix_transform_rule", fieldType:goog.proto2
.Message.FieldType.STRING, type:String}, 18:{name:"same_mobile_and_fixed_line_pattern", fieldType:goog.proto2.Message.FieldType.
BOOL, defaultValue:!1, type:Boolean}, 19:{name:"number_format", repeated:!0, fieldType:goog.proto2.Message.FieldType.MESSAGE,
  type:i18n.phonenumbers.NumberFormat}, 20:{name:"intl_number_format", repeated:!0, fieldType:goog.proto2.Message.FieldType.MESSAGE
, type:i18n.phonenumbers.NumberFormat}, 22:{name:"main_country_for_code", fieldType:goog.proto2.Message.FieldType.BOOL, defaultValue
:!1, type:Boolean}, 23:{name:"leading_digits", fieldType:goog.proto2.Message.FieldType.STRING, type:String}, 26:{name:"leading_zero_possible
", fieldType:goog.proto2.Message.FieldType.BOOL, defaultValue:!1, type:Boolean}}));
  return a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getEmergency"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getEmergency ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getEmergency)
- description and source-code
```javascript
getEmergency = function () {
  return this.get$Value(27);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getEmergencyOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getEmergencyOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getEmergencyOrDefault)
- description and source-code
```javascript
getEmergencyOrDefault = function () {
  return this.get$ValueOrDefault(27);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getFixedLine"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getFixedLine ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getFixedLine)
- description and source-code
```javascript
getFixedLine = function () {
  return this.get$Value(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getFixedLineOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getFixedLineOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getFixedLineOrDefault)
- description and source-code
```javascript
getFixedLineOrDefault = function () {
  return this.get$ValueOrDefault(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getGeneralDesc"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getGeneralDesc ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getGeneralDesc)
- description and source-code
```javascript
getGeneralDesc = function () {
  return this.get$Value(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getGeneralDescOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getGeneralDescOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getGeneralDescOrDefault)
- description and source-code
```javascript
getGeneralDescOrDefault = function () {
  return this.get$ValueOrDefault(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getId"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getId ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getId)
- description and source-code
```javascript
getId = function () {
  return this.get$Value(9);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getIdOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getIdOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getIdOrDefault)
- description and source-code
```javascript
getIdOrDefault = function () {
  return this.get$ValueOrDefault(9);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getInternationalPrefix"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getInternationalPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getInternationalPrefix)
- description and source-code
```javascript
getInternationalPrefix = function () {
  return this.get$Value(11);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getInternationalPrefixOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getInternationalPrefixOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getInternationalPrefixOrDefault)
- description and source-code
```javascript
getInternationalPrefixOrDefault = function () {
  return this.get$ValueOrDefault(11);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getIntlNumberFormat"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getIntlNumberFormat (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getIntlNumberFormat)
- description and source-code
```javascript
getIntlNumberFormat = function (a) {
  return this.get$Value(20, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getIntlNumberFormatOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getIntlNumberFormatOrDefault (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getIntlNumberFormatOrDefault)
- description and source-code
```javascript
getIntlNumberFormatOrDefault = function (a) {
  return this.get$ValueOrDefault(20, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getLeadingDigits"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getLeadingDigits ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getLeadingDigits)
- description and source-code
```javascript
getLeadingDigits = function () {
  return this.get$Value(23);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getLeadingDigitsOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getLeadingDigitsOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getLeadingDigitsOrDefault)
- description and source-code
```javascript
getLeadingDigitsOrDefault = function () {
  return this.get$ValueOrDefault(23);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getLeadingZeroPossible"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getLeadingZeroPossible ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getLeadingZeroPossible)
- description and source-code
```javascript
getLeadingZeroPossible = function () {
  return this.get$Value(26);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getLeadingZeroPossibleOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getLeadingZeroPossibleOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getLeadingZeroPossibleOrDefault)
- description and source-code
```javascript
getLeadingZeroPossibleOrDefault = function () {
  return this.get$ValueOrDefault(26);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getMainCountryForCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getMainCountryForCode ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getMainCountryForCode)
- description and source-code
```javascript
getMainCountryForCode = function () {
  return this.get$Value(22);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getMainCountryForCodeOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getMainCountryForCodeOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getMainCountryForCodeOrDefault)
- description and source-code
```javascript
getMainCountryForCodeOrDefault = function () {
  return this.get$ValueOrDefault(22);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getMobile"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getMobile ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getMobile)
- description and source-code
```javascript
getMobile = function () {
  return this.get$Value(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getMobileOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getMobileOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getMobileOrDefault)
- description and source-code
```javascript
getMobileOrDefault = function () {
  return this.get$ValueOrDefault(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNationalPrefix"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNationalPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNationalPrefix)
- description and source-code
```javascript
getNationalPrefix = function () {
  return this.get$Value(12);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNationalPrefixForParsing"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNationalPrefixForParsing ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNationalPrefixForParsing)
- description and source-code
```javascript
getNationalPrefixForParsing = function () {
  return this.get$Value(15);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNationalPrefixForParsingOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNationalPrefixForParsingOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNationalPrefixForParsingOrDefault)
- description and source-code
```javascript
getNationalPrefixForParsingOrDefault = function () {
  return this.get$ValueOrDefault(15);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNationalPrefixOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNationalPrefixOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNationalPrefixOrDefault)
- description and source-code
```javascript
getNationalPrefixOrDefault = function () {
  return this.get$ValueOrDefault(12);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNationalPrefixTransformRule"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNationalPrefixTransformRule ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNationalPrefixTransformRule)
- description and source-code
```javascript
getNationalPrefixTransformRule = function () {
  return this.get$Value(16);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNationalPrefixTransformRuleOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNationalPrefixTransformRuleOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNationalPrefixTransformRuleOrDefault)
- description and source-code
```javascript
getNationalPrefixTransformRuleOrDefault = function () {
  return this.get$ValueOrDefault(16);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNoInternationalDialling"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNoInternationalDialling ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNoInternationalDialling)
- description and source-code
```javascript
getNoInternationalDialling = function () {
  return this.get$Value(24);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNoInternationalDiallingOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNoInternationalDiallingOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNoInternationalDiallingOrDefault)
- description and source-code
```javascript
getNoInternationalDiallingOrDefault = function () {
  return this.get$ValueOrDefault(24);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNumberFormat"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNumberFormat (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNumberFormat)
- description and source-code
```javascript
getNumberFormat = function (a) {
  return this.get$Value(19, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNumberFormatOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getNumberFormatOrDefault (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getNumberFormatOrDefault)
- description and source-code
```javascript
getNumberFormatOrDefault = function (a) {
  return this.get$ValueOrDefault(19, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPager"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPager ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPager)
- description and source-code
```javascript
getPager = function () {
  return this.get$Value(21);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPagerOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPagerOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPagerOrDefault)
- description and source-code
```javascript
getPagerOrDefault = function () {
  return this.get$ValueOrDefault(21);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPersonalNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPersonalNumber ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPersonalNumber)
- description and source-code
```javascript
getPersonalNumber = function () {
  return this.get$Value(7);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPersonalNumberOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPersonalNumberOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPersonalNumberOrDefault)
- description and source-code
```javascript
getPersonalNumberOrDefault = function () {
  return this.get$ValueOrDefault(7);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPreferredExtnPrefix"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPreferredExtnPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPreferredExtnPrefix)
- description and source-code
```javascript
getPreferredExtnPrefix = function () {
  return this.get$Value(13);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPreferredExtnPrefixOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPreferredExtnPrefixOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPreferredExtnPrefixOrDefault)
- description and source-code
```javascript
getPreferredExtnPrefixOrDefault = function () {
  return this.get$ValueOrDefault(13);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPreferredInternationalPrefix"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPreferredInternationalPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPreferredInternationalPrefix)
- description and source-code
```javascript
getPreferredInternationalPrefix = function () {
  return this.get$Value(17);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPreferredInternationalPrefixOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPreferredInternationalPrefixOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPreferredInternationalPrefixOrDefault)
- description and source-code
```javascript
getPreferredInternationalPrefixOrDefault = function () {
  return this.get$ValueOrDefault(17);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPremiumRate"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPremiumRate ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPremiumRate)
- description and source-code
```javascript
getPremiumRate = function () {
  return this.get$Value(5);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPremiumRateOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getPremiumRateOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getPremiumRateOrDefault)
- description and source-code
```javascript
getPremiumRateOrDefault = function () {
  return this.get$ValueOrDefault(5);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getSameMobileAndFixedLinePattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getSameMobileAndFixedLinePattern ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getSameMobileAndFixedLinePattern)
- description and source-code
```javascript
getSameMobileAndFixedLinePattern = function () {
  return this.get$Value(18);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getSameMobileAndFixedLinePatternOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getSameMobileAndFixedLinePatternOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getSameMobileAndFixedLinePatternOrDefault)
- description and source-code
```javascript
getSameMobileAndFixedLinePatternOrDefault = function () {
  return this.get$ValueOrDefault(18);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getSharedCost"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getSharedCost ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getSharedCost)
- description and source-code
```javascript
getSharedCost = function () {
  return this.get$Value(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getSharedCostOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getSharedCostOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getSharedCostOrDefault)
- description and source-code
```javascript
getSharedCostOrDefault = function () {
  return this.get$ValueOrDefault(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getTollFree"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getTollFree ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getTollFree)
- description and source-code
```javascript
getTollFree = function () {
  return this.get$Value(4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getTollFreeOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getTollFreeOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getTollFreeOrDefault)
- description and source-code
```javascript
getTollFreeOrDefault = function () {
  return this.get$ValueOrDefault(4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getUan"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getUan ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getUan)
- description and source-code
```javascript
getUan = function () {
  return this.get$Value(25);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getUanOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getUanOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getUanOrDefault)
- description and source-code
```javascript
getUanOrDefault = function () {
  return this.get$ValueOrDefault(25);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getVoicemail"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getVoicemail ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getVoicemail)
- description and source-code
```javascript
getVoicemail = function () {
  return this.get$Value(28);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getVoicemailOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getVoicemailOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getVoicemailOrDefault)
- description and source-code
```javascript
getVoicemailOrDefault = function () {
  return this.get$ValueOrDefault(28);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getVoip"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getVoip ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getVoip)
- description and source-code
```javascript
getVoip = function () {
  return this.get$Value(8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getVoipOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>getVoipOrDefault ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.getVoipOrDefault)
- description and source-code
```javascript
getVoipOrDefault = function () {
  return this.get$ValueOrDefault(8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasCountryCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasCountryCode ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasCountryCode)
- description and source-code
```javascript
hasCountryCode = function () {
  return this.has$Value(10);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasEmergency"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasEmergency ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasEmergency)
- description and source-code
```javascript
hasEmergency = function () {
  return this.has$Value(27);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasFixedLine"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasFixedLine ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasFixedLine)
- description and source-code
```javascript
hasFixedLine = function () {
  return this.has$Value(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasGeneralDesc"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasGeneralDesc ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasGeneralDesc)
- description and source-code
```javascript
hasGeneralDesc = function () {
  return this.has$Value(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasId"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasId ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasId)
- description and source-code
```javascript
hasId = function () {
  return this.has$Value(9);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasInternationalPrefix"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasInternationalPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasInternationalPrefix)
- description and source-code
```javascript
hasInternationalPrefix = function () {
  return this.has$Value(11);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasIntlNumberFormat"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasIntlNumberFormat ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasIntlNumberFormat)
- description and source-code
```javascript
hasIntlNumberFormat = function () {
  return this.has$Value(20);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasLeadingDigits"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasLeadingDigits ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasLeadingDigits)
- description and source-code
```javascript
hasLeadingDigits = function () {
  return this.has$Value(23);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasLeadingZeroPossible"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasLeadingZeroPossible ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasLeadingZeroPossible)
- description and source-code
```javascript
hasLeadingZeroPossible = function () {
  return this.has$Value(26);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasMainCountryForCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasMainCountryForCode ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasMainCountryForCode)
- description and source-code
```javascript
hasMainCountryForCode = function () {
  return this.has$Value(22);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasMobile"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasMobile ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasMobile)
- description and source-code
```javascript
hasMobile = function () {
  return this.has$Value(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasNationalPrefix"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasNationalPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasNationalPrefix)
- description and source-code
```javascript
hasNationalPrefix = function () {
  return this.has$Value(12);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasNationalPrefixForParsing"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasNationalPrefixForParsing ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasNationalPrefixForParsing)
- description and source-code
```javascript
hasNationalPrefixForParsing = function () {
  return this.has$Value(15);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasNationalPrefixTransformRule"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasNationalPrefixTransformRule ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasNationalPrefixTransformRule)
- description and source-code
```javascript
hasNationalPrefixTransformRule = function () {
  return this.has$Value(16);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasNoInternationalDialling"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasNoInternationalDialling ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasNoInternationalDialling)
- description and source-code
```javascript
hasNoInternationalDialling = function () {
  return this.has$Value(24);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasNumberFormat"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasNumberFormat ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasNumberFormat)
- description and source-code
```javascript
hasNumberFormat = function () {
  return this.has$Value(19);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasPager"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasPager ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasPager)
- description and source-code
```javascript
hasPager = function () {
  return this.has$Value(21);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasPersonalNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasPersonalNumber ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasPersonalNumber)
- description and source-code
```javascript
hasPersonalNumber = function () {
  return this.has$Value(7);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasPreferredExtnPrefix"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasPreferredExtnPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasPreferredExtnPrefix)
- description and source-code
```javascript
hasPreferredExtnPrefix = function () {
  return this.has$Value(13);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasPreferredInternationalPrefix"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasPreferredInternationalPrefix ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasPreferredInternationalPrefix)
- description and source-code
```javascript
hasPreferredInternationalPrefix = function () {
  return this.has$Value(17);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasPremiumRate"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasPremiumRate ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasPremiumRate)
- description and source-code
```javascript
hasPremiumRate = function () {
  return this.has$Value(5);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasSameMobileAndFixedLinePattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasSameMobileAndFixedLinePattern ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasSameMobileAndFixedLinePattern)
- description and source-code
```javascript
hasSameMobileAndFixedLinePattern = function () {
  return this.has$Value(18);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasSharedCost"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasSharedCost ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasSharedCost)
- description and source-code
```javascript
hasSharedCost = function () {
  return this.has$Value(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasTollFree"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasTollFree ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasTollFree)
- description and source-code
```javascript
hasTollFree = function () {
  return this.has$Value(4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasUan"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasUan ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasUan)
- description and source-code
```javascript
hasUan = function () {
  return this.has$Value(25);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasVoicemail"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasVoicemail ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasVoicemail)
- description and source-code
```javascript
hasVoicemail = function () {
  return this.has$Value(28);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasVoip"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>hasVoip ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.hasVoip)
- description and source-code
```javascript
hasVoip = function () {
  return this.has$Value(8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.idCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>idCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.idCount)
- description and source-code
```javascript
idCount = function () {
  return this.count$Values(9);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.internationalPrefixCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>internationalPrefixCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.internationalPrefixCount)
- description and source-code
```javascript
internationalPrefixCount = function () {
  return this.count$Values(11);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.intlNumberFormatArray"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>intlNumberFormatArray ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.intlNumberFormatArray)
- description and source-code
```javascript
intlNumberFormatArray = function () {
  return this.array$Values(20);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.intlNumberFormatCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>intlNumberFormatCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.intlNumberFormatCount)
- description and source-code
```javascript
intlNumberFormatCount = function () {
  return this.count$Values(20);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.leadingDigitsCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>leadingDigitsCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.leadingDigitsCount)
- description and source-code
```javascript
leadingDigitsCount = function () {
  return this.count$Values(23);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.leadingZeroPossibleCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>leadingZeroPossibleCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.leadingZeroPossibleCount)
- description and source-code
```javascript
leadingZeroPossibleCount = function () {
  return this.count$Values(26);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.mainCountryForCodeCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>mainCountryForCodeCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.mainCountryForCodeCount)
- description and source-code
```javascript
mainCountryForCodeCount = function () {
  return this.count$Values(22);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.mobileCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>mobileCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.mobileCount)
- description and source-code
```javascript
mobileCount = function () {
  return this.count$Values(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.nationalPrefixCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>nationalPrefixCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.nationalPrefixCount)
- description and source-code
```javascript
nationalPrefixCount = function () {
  return this.count$Values(12);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.nationalPrefixForParsingCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>nationalPrefixForParsingCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.nationalPrefixForParsingCount)
- description and source-code
```javascript
nationalPrefixForParsingCount = function () {
  return this.count$Values(15);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.nationalPrefixTransformRuleCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>nationalPrefixTransformRuleCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.nationalPrefixTransformRuleCount)
- description and source-code
```javascript
nationalPrefixTransformRuleCount = function () {
  return this.count$Values(16);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.noInternationalDiallingCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>noInternationalDiallingCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.noInternationalDiallingCount)
- description and source-code
```javascript
noInternationalDiallingCount = function () {
  return this.count$Values(24);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.numberFormatArray"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>numberFormatArray ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.numberFormatArray)
- description and source-code
```javascript
numberFormatArray = function () {
  return this.array$Values(19);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.numberFormatCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>numberFormatCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.numberFormatCount)
- description and source-code
```javascript
numberFormatCount = function () {
  return this.count$Values(19);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.pagerCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>pagerCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.pagerCount)
- description and source-code
```javascript
pagerCount = function () {
  return this.count$Values(21);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.personalNumberCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>personalNumberCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.personalNumberCount)
- description and source-code
```javascript
personalNumberCount = function () {
  return this.count$Values(7);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.preferredExtnPrefixCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>preferredExtnPrefixCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.preferredExtnPrefixCount)
- description and source-code
```javascript
preferredExtnPrefixCount = function () {
  return this.count$Values(13);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.preferredInternationalPrefixCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>preferredInternationalPrefixCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.preferredInternationalPrefixCount)
- description and source-code
```javascript
preferredInternationalPrefixCount = function () {
  return this.count$Values(17);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.premiumRateCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>premiumRateCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.premiumRateCount)
- description and source-code
```javascript
premiumRateCount = function () {
  return this.count$Values(5);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.sameMobileAndFixedLinePatternCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>sameMobileAndFixedLinePatternCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.sameMobileAndFixedLinePatternCount)
- description and source-code
```javascript
sameMobileAndFixedLinePatternCount = function () {
  return this.count$Values(18);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setCountryCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setCountryCode (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setCountryCode)
- description and source-code
```javascript
setCountryCode = function (a) {
  this.set$Value(10, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setEmergency"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setEmergency (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setEmergency)
- description and source-code
```javascript
setEmergency = function (a) {
  this.set$Value(27, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setFixedLine"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setFixedLine (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setFixedLine)
- description and source-code
```javascript
setFixedLine = function (a) {
  this.set$Value(2, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setGeneralDesc"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setGeneralDesc (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setGeneralDesc)
- description and source-code
```javascript
setGeneralDesc = function (a) {
  this.set$Value(1, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setId"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setId (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setId)
- description and source-code
```javascript
setId = function (a) {
  this.set$Value(9, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setInternationalPrefix"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setInternationalPrefix (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setInternationalPrefix)
- description and source-code
```javascript
setInternationalPrefix = function (a) {
  this.set$Value(11, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setLeadingDigits"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setLeadingDigits (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setLeadingDigits)
- description and source-code
```javascript
setLeadingDigits = function (a) {
  this.set$Value(23, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setLeadingZeroPossible"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setLeadingZeroPossible (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setLeadingZeroPossible)
- description and source-code
```javascript
setLeadingZeroPossible = function (a) {
  this.set$Value(26, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setMainCountryForCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setMainCountryForCode (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setMainCountryForCode)
- description and source-code
```javascript
setMainCountryForCode = function (a) {
  this.set$Value(22, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setMobile"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setMobile (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setMobile)
- description and source-code
```javascript
setMobile = function (a) {
  this.set$Value(3, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setNationalPrefix"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setNationalPrefix (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setNationalPrefix)
- description and source-code
```javascript
setNationalPrefix = function (a) {
  this.set$Value(12, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setNationalPrefixForParsing"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setNationalPrefixForParsing (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setNationalPrefixForParsing)
- description and source-code
```javascript
setNationalPrefixForParsing = function (a) {
  this.set$Value(15, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setNationalPrefixTransformRule"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setNationalPrefixTransformRule (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setNationalPrefixTransformRule)
- description and source-code
```javascript
setNationalPrefixTransformRule = function (a) {
  this.set$Value(16, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setNoInternationalDialling"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setNoInternationalDialling (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setNoInternationalDialling)
- description and source-code
```javascript
setNoInternationalDialling = function (a) {
  this.set$Value(24, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setPager"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setPager (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setPager)
- description and source-code
```javascript
setPager = function (a) {
  this.set$Value(21, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setPersonalNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setPersonalNumber (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setPersonalNumber)
- description and source-code
```javascript
setPersonalNumber = function (a) {
  this.set$Value(7, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setPreferredExtnPrefix"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setPreferredExtnPrefix (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setPreferredExtnPrefix)
- description and source-code
```javascript
setPreferredExtnPrefix = function (a) {
  this.set$Value(13, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setPreferredInternationalPrefix"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setPreferredInternationalPrefix (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setPreferredInternationalPrefix)
- description and source-code
```javascript
setPreferredInternationalPrefix = function (a) {
  this.set$Value(17, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setPremiumRate"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setPremiumRate (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setPremiumRate)
- description and source-code
```javascript
setPremiumRate = function (a) {
  this.set$Value(5, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setSameMobileAndFixedLinePattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setSameMobileAndFixedLinePattern (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setSameMobileAndFixedLinePattern)
- description and source-code
```javascript
setSameMobileAndFixedLinePattern = function (a) {
  this.set$Value(18, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setSharedCost"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setSharedCost (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setSharedCost)
- description and source-code
```javascript
setSharedCost = function (a) {
  this.set$Value(6, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setTollFree"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setTollFree (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setTollFree)
- description and source-code
```javascript
setTollFree = function (a) {
  this.set$Value(4, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setUan"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setUan (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setUan)
- description and source-code
```javascript
setUan = function (a) {
  this.set$Value(25, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setVoicemail"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setVoicemail (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setVoicemail)
- description and source-code
```javascript
setVoicemail = function (a) {
  this.set$Value(28, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setVoip"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>setVoip (a)](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.setVoip)
- description and source-code
```javascript
setVoip = function (a) {
  this.set$Value(8, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.sharedCostCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>sharedCostCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.sharedCostCount)
- description and source-code
```javascript
sharedCostCount = function () {
  return this.count$Values(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.tollFreeCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>tollFreeCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.tollFreeCount)
- description and source-code
```javascript
tollFreeCount = function () {
  return this.count$Values(4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.uanCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>uanCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.uanCount)
- description and source-code
```javascript
uanCount = function () {
  return this.count$Values(25);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.voicemailCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>voicemailCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.voicemailCount)
- description and source-code
```javascript
voicemailCount = function () {
  return this.count$Values(28);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadata.prototype.voipCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadata.prototype.</span>voipCount ()](#apidoc.element.google-libphonenumber.PhoneMetadata.prototype.voipCount)
- description and source-code
```javascript
voipCount = function () {
  return this.count$Values(8);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.google-libphonenumber.PhoneMetadataCollection"></a>[module google-libphonenumber.PhoneMetadataCollection](#apidoc.module.google-libphonenumber.PhoneMetadataCollection)

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadataCollection.PhoneMetadataCollection"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneMetadataCollection ()](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.PhoneMetadataCollection)
- description and source-code
```javascript
PhoneMetadataCollection = function () {
  goog.proto2.Message.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadataCollection.base"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.</span>base (a, c, f)](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.base)
- description and source-code
```javascript
base = function (a, c, f) {
  for (var d = Array(arguments.length - 2), e = 2;e < arguments.length;e++) {
    d[e - 2] = arguments[e];
  }
  return b.prototype[c].apply(a, d);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadataCollection.getDescriptor"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.getDescriptor)
- description and source-code
```javascript
getDescriptor = function () {
  var a = i18n.phonenumbers.PhoneMetadataCollection.descriptor_;
  a || (i18n.phonenumbers.PhoneMetadataCollection.descriptor_ = a = goog.proto2.Message.createDescriptor(i18n.phonenumbers.PhoneMetadataCollection
, {0:{name:"PhoneMetadataCollection", fullName:"i18n.phonenumbers.PhoneMetadataCollection"}, 1:{name:"metadata", repeated:!0, fieldType
:goog.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneMetadata}}));
  return a;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.google-libphonenumber.PhoneMetadataCollection.prototype"></a>[module google-libphonenumber.PhoneMetadataCollection.prototype](#apidoc.module.google-libphonenumber.PhoneMetadataCollection.prototype)

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.addMetadata"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.prototype.</span>addMetadata (a)](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.addMetadata)
- description and source-code
```javascript
addMetadata = function (a) {
  this.add$Value(1, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.clearMetadata"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.prototype.</span>clearMetadata ()](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.clearMetadata)
- description and source-code
```javascript
clearMetadata = function () {
  this.clear$Field(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.constructor"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.prototype.</span>constructor ()](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  goog.proto2.Message.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.getDescriptor"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.prototype.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.getDescriptor)
- description and source-code
```javascript
getDescriptor = function () {
  var a = i18n.phonenumbers.PhoneMetadataCollection.descriptor_;
  a || (i18n.phonenumbers.PhoneMetadataCollection.descriptor_ = a = goog.proto2.Message.createDescriptor(i18n.phonenumbers.PhoneMetadataCollection
, {0:{name:"PhoneMetadataCollection", fullName:"i18n.phonenumbers.PhoneMetadataCollection"}, 1:{name:"metadata", repeated:!0, fieldType
:goog.proto2.Message.FieldType.MESSAGE, type:i18n.phonenumbers.PhoneMetadata}}));
  return a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.getMetadata"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.prototype.</span>getMetadata (a)](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.getMetadata)
- description and source-code
```javascript
getMetadata = function (a) {
  return this.get$Value(1, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.getMetadataOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.prototype.</span>getMetadataOrDefault (a)](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.getMetadataOrDefault)
- description and source-code
```javascript
getMetadataOrDefault = function (a) {
  return this.get$ValueOrDefault(1, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.hasMetadata"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.prototype.</span>hasMetadata ()](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.hasMetadata)
- description and source-code
```javascript
hasMetadata = function () {
  return this.has$Value(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.metadataArray"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.prototype.</span>metadataArray ()](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.metadataArray)
- description and source-code
```javascript
metadataArray = function () {
  return this.array$Values(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.metadataCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneMetadataCollection.prototype.</span>metadataCount ()](#apidoc.element.google-libphonenumber.PhoneMetadataCollection.prototype.metadataCount)
- description and source-code
```javascript
metadataCount = function () {
  return this.count$Values(1);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.google-libphonenumber.PhoneNumber"></a>[module google-libphonenumber.PhoneNumber](#apidoc.module.google-libphonenumber.PhoneNumber)

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.PhoneNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneNumber ()](#apidoc.element.google-libphonenumber.PhoneNumber.PhoneNumber)
- description and source-code
```javascript
PhoneNumber = function () {
  goog.proto2.Message.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.base"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.</span>base (a, c, f)](#apidoc.element.google-libphonenumber.PhoneNumber.base)
- description and source-code
```javascript
base = function (a, c, f) {
  for (var d = Array(arguments.length - 2), e = 2;e < arguments.length;e++) {
    d[e - 2] = arguments[e];
  }
  return b.prototype[c].apply(a, d);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.ctor"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.</span>ctor ()](#apidoc.element.google-libphonenumber.PhoneNumber.ctor)
- description and source-code
```javascript
ctor = function () {
  goog.proto2.Message.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.getDescriptor"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.PhoneNumber.getDescriptor)
- description and source-code
```javascript
getDescriptor = function () {
  i18n.phonenumbers.PhoneNumber.descriptor_ || (i18n.phonenumbers.PhoneNumber.descriptor_ = goog.proto2.Message.createDescriptor
(i18n.phonenumbers.PhoneNumber, {0:{name:"PhoneNumber", fullName:"i18n.phonenumbers.PhoneNumber"}, 1:{name:"country_code", required
:!0, fieldType:goog.proto2.Message.FieldType.INT32, type:Number}, 2:{name:"national_number", required:!0, fieldType:goog.proto2.
Message.FieldType.UINT64, type:Number}, 3:{name:"extension", fieldType:goog.proto2.Message.FieldType.STRING, type:String},
  4:{name:"italian_leading_zero", fieldType:goog.proto2.Message.FieldType.BOOL, type:Boolean}, 8:{name:"number_of_leading_zeros",
fieldType:goog.proto2.Message.FieldType.INT32, defaultValue:1, type:Number}, 5:{name:"raw_input", fieldType:goog.proto2.Message.
FieldType.STRING, type:String}, 6:{name:"country_code_source", fieldType:goog.proto2.Message.FieldType.ENUM, defaultValue:i18n.phonenumbers
.PhoneNumber.CountryCodeSource.FROM_NUMBER_WITH_PLUS_SIGN, type:i18n.phonenumbers.PhoneNumber.CountryCodeSource},
  7:{name:"preferred_domestic_carrier_code", fieldType:goog.proto2.Message.FieldType.STRING, type:String}}));
  return i18n.phonenumbers.PhoneNumber.descriptor_;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.google-libphonenumber.PhoneNumber.prototype"></a>[module google-libphonenumber.PhoneNumber.prototype](#apidoc.module.google-libphonenumber.PhoneNumber.prototype)

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearCountryCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>clearCountryCode ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearCountryCode)
- description and source-code
```javascript
clearCountryCode = function () {
  this.clear$Field(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearCountryCodeSource"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>clearCountryCodeSource ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearCountryCodeSource)
- description and source-code
```javascript
clearCountryCodeSource = function () {
  this.clear$Field(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearExtension"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>clearExtension ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearExtension)
- description and source-code
```javascript
clearExtension = function () {
  this.clear$Field(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearItalianLeadingZero"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>clearItalianLeadingZero ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearItalianLeadingZero)
- description and source-code
```javascript
clearItalianLeadingZero = function () {
  this.clear$Field(4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearNationalNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>clearNationalNumber ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearNationalNumber)
- description and source-code
```javascript
clearNationalNumber = function () {
  this.clear$Field(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearNumberOfLeadingZeros"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>clearNumberOfLeadingZeros ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearNumberOfLeadingZeros)
- description and source-code
```javascript
clearNumberOfLeadingZeros = function () {
  this.clear$Field(8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearPreferredDomesticCarrierCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>clearPreferredDomesticCarrierCode ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearPreferredDomesticCarrierCode)
- description and source-code
```javascript
clearPreferredDomesticCarrierCode = function () {
  this.clear$Field(7);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearRawInput"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>clearRawInput ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.clearRawInput)
- description and source-code
```javascript
clearRawInput = function () {
  this.clear$Field(5);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.constructor"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>constructor ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  goog.proto2.Message.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.countryCodeCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>countryCodeCount ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.countryCodeCount)
- description and source-code
```javascript
countryCodeCount = function () {
  return this.count$Values(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.countryCodeSourceCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>countryCodeSourceCount ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.countryCodeSourceCount)
- description and source-code
```javascript
countryCodeSourceCount = function () {
  return this.count$Values(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.extensionCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>extensionCount ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.extensionCount)
- description and source-code
```javascript
extensionCount = function () {
  return this.count$Values(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.getCountryCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getCountryCode ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getCountryCode)
- description and source-code
```javascript
getCountryCode = function () {
  return this.get$Value(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.getCountryCodeOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getCountryCodeOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getCountryCodeOrDefault)
- description and source-code
```javascript
getCountryCodeOrDefault = function () {
  return this.get$ValueOrDefault(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.getCountryCodeSource"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getCountryCodeSource ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getCountryCodeSource)
- description and source-code
```javascript
getCountryCodeSource = function () {
  return this.get$Value(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.getCountryCodeSourceOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getCountryCodeSourceOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getCountryCodeSourceOrDefault)
- description and source-code
```javascript
getCountryCodeSourceOrDefault = function () {
  return this.get$ValueOrDefault(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.getDescriptor"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getDescriptor)
- description and source-code
```javascript
getDescriptor = function () {
  i18n.phonenumbers.PhoneNumber.descriptor_ || (i18n.phonenumbers.PhoneNumber.descriptor_ = goog.proto2.Message.createDescriptor
(i18n.phonenumbers.PhoneNumber, {0:{name:"PhoneNumber", fullName:"i18n.phonenumbers.PhoneNumber"}, 1:{name:"country_code", required
:!0, fieldType:goog.proto2.Message.FieldType.INT32, type:Number}, 2:{name:"national_number", required:!0, fieldType:goog.proto2.
Message.FieldType.UINT64, type:Number}, 3:{name:"extension", fieldType:goog.proto2.Message.FieldType.STRING, type:String},
  4:{name:"italian_leading_zero", fieldType:goog.proto2.Message.FieldType.BOOL, type:Boolean}, 8:{name:"number_of_leading_zeros",
fieldType:goog.proto2.Message.FieldType.INT32, defaultValue:1, type:Number}, 5:{name:"raw_input", fieldType:goog.proto2.Message.
FieldType.STRING, type:String}, 6:{name:"country_code_source", fieldType:goog.proto2.Message.FieldType.ENUM, defaultValue:i18n.phonenumbers
.PhoneNumber.CountryCodeSource.FROM_NUMBER_WITH_PLUS_SIGN, type:i18n.phonenumbers.PhoneNumber.CountryCodeSource},
  7:{name:"preferred_domestic_carrier_code", fieldType:goog.proto2.Message.FieldType.STRING, type:String}}));
  return i18n.phonenumbers.PhoneNumber.descriptor_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.getExtension"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getExtension ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getExtension)
- description and source-code
```javascript
getExtension = function () {
  return this.get$Value(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.getExtensionOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getExtensionOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getExtensionOrDefault)
- description and source-code
```javascript
getExtensionOrDefault = function () {
  return this.get$ValueOrDefault(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.getItalianLeadingZero"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getItalianLeadingZero ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getItalianLeadingZero)
- description and source-code
```javascript
getItalianLeadingZero = function () {
  return this.get$Value(4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.getItalianLeadingZeroOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getItalianLeadingZeroOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getItalianLeadingZeroOrDefault)
- description and source-code
```javascript
getItalianLeadingZeroOrDefault = function () {
  return this.get$ValueOrDefault(4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.getNationalNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getNationalNumber ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getNationalNumber)
- description and source-code
```javascript
getNationalNumber = function () {
  return this.get$Value(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.getNationalNumberOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getNationalNumberOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getNationalNumberOrDefault)
- description and source-code
```javascript
getNationalNumberOrDefault = function () {
  return this.get$ValueOrDefault(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.getNumberOfLeadingZeros"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getNumberOfLeadingZeros ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getNumberOfLeadingZeros)
- description and source-code
```javascript
getNumberOfLeadingZeros = function () {
  return this.get$Value(8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.getNumberOfLeadingZerosOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getNumberOfLeadingZerosOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getNumberOfLeadingZerosOrDefault)
- description and source-code
```javascript
getNumberOfLeadingZerosOrDefault = function () {
  return this.get$ValueOrDefault(8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.getPreferredDomesticCarrierCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getPreferredDomesticCarrierCode ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getPreferredDomesticCarrierCode)
- description and source-code
```javascript
getPreferredDomesticCarrierCode = function () {
  return this.get$Value(7);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.getPreferredDomesticCarrierCodeOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getPreferredDomesticCarrierCodeOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getPreferredDomesticCarrierCodeOrDefault)
- description and source-code
```javascript
getPreferredDomesticCarrierCodeOrDefault = function () {
  return this.get$ValueOrDefault(7);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.getRawInput"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getRawInput ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getRawInput)
- description and source-code
```javascript
getRawInput = function () {
  return this.get$Value(5);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.getRawInputOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>getRawInputOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.getRawInputOrDefault)
- description and source-code
```javascript
getRawInputOrDefault = function () {
  return this.get$ValueOrDefault(5);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasCountryCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>hasCountryCode ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasCountryCode)
- description and source-code
```javascript
hasCountryCode = function () {
  return this.has$Value(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasCountryCodeSource"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>hasCountryCodeSource ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasCountryCodeSource)
- description and source-code
```javascript
hasCountryCodeSource = function () {
  return this.has$Value(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasExtension"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>hasExtension ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasExtension)
- description and source-code
```javascript
hasExtension = function () {
  return this.has$Value(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasItalianLeadingZero"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>hasItalianLeadingZero ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasItalianLeadingZero)
- description and source-code
```javascript
hasItalianLeadingZero = function () {
  return this.has$Value(4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasNationalNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>hasNationalNumber ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasNationalNumber)
- description and source-code
```javascript
hasNationalNumber = function () {
  return this.has$Value(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasNumberOfLeadingZeros"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>hasNumberOfLeadingZeros ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasNumberOfLeadingZeros)
- description and source-code
```javascript
hasNumberOfLeadingZeros = function () {
  return this.has$Value(8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasPreferredDomesticCarrierCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>hasPreferredDomesticCarrierCode ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasPreferredDomesticCarrierCode)
- description and source-code
```javascript
hasPreferredDomesticCarrierCode = function () {
  return this.has$Value(7);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasRawInput"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>hasRawInput ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.hasRawInput)
- description and source-code
```javascript
hasRawInput = function () {
  return this.has$Value(5);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.italianLeadingZeroCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>italianLeadingZeroCount ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.italianLeadingZeroCount)
- description and source-code
```javascript
italianLeadingZeroCount = function () {
  return this.count$Values(4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.nationalNumberCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>nationalNumberCount ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.nationalNumberCount)
- description and source-code
```javascript
nationalNumberCount = function () {
  return this.count$Values(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.numberOfLeadingZerosCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>numberOfLeadingZerosCount ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.numberOfLeadingZerosCount)
- description and source-code
```javascript
numberOfLeadingZerosCount = function () {
  return this.count$Values(8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.preferredDomesticCarrierCodeCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>preferredDomesticCarrierCodeCount ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.preferredDomesticCarrierCodeCount)
- description and source-code
```javascript
preferredDomesticCarrierCodeCount = function () {
  return this.count$Values(7);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.rawInputCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>rawInputCount ()](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.rawInputCount)
- description and source-code
```javascript
rawInputCount = function () {
  return this.count$Values(5);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.setCountryCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>setCountryCode (a)](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.setCountryCode)
- description and source-code
```javascript
setCountryCode = function (a) {
  this.set$Value(1, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.setCountryCodeSource"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>setCountryCodeSource (a)](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.setCountryCodeSource)
- description and source-code
```javascript
setCountryCodeSource = function (a) {
  this.set$Value(6, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.setExtension"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>setExtension (a)](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.setExtension)
- description and source-code
```javascript
setExtension = function (a) {
  this.set$Value(3, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.setItalianLeadingZero"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>setItalianLeadingZero (a)](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.setItalianLeadingZero)
- description and source-code
```javascript
setItalianLeadingZero = function (a) {
  this.set$Value(4, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.setNationalNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>setNationalNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.setNationalNumber)
- description and source-code
```javascript
setNationalNumber = function (a) {
  this.set$Value(2, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.setNumberOfLeadingZeros"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>setNumberOfLeadingZeros (a)](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.setNumberOfLeadingZeros)
- description and source-code
```javascript
setNumberOfLeadingZeros = function (a) {
  this.set$Value(8, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.setPreferredDomesticCarrierCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>setPreferredDomesticCarrierCode (a)](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.setPreferredDomesticCarrierCode)
- description and source-code
```javascript
setPreferredDomesticCarrierCode = function (a) {
  this.set$Value(7, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumber.prototype.setRawInput"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumber.prototype.</span>setRawInput (a)](#apidoc.element.google-libphonenumber.PhoneNumber.prototype.setRawInput)
- description and source-code
```javascript
setRawInput = function (a) {
  this.set$Value(5, a);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.google-libphonenumber.PhoneNumberDesc"></a>[module google-libphonenumber.PhoneNumberDesc](#apidoc.module.google-libphonenumber.PhoneNumberDesc)

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.PhoneNumberDesc"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneNumberDesc ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.PhoneNumberDesc)
- description and source-code
```javascript
PhoneNumberDesc = function () {
  goog.proto2.Message.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.base"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.</span>base (a, c, f)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.base)
- description and source-code
```javascript
base = function (a, c, f) {
  for (var d = Array(arguments.length - 2), e = 2;e < arguments.length;e++) {
    d[e - 2] = arguments[e];
  }
  return b.prototype[c].apply(a, d);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.getDescriptor"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.getDescriptor)
- description and source-code
```javascript
getDescriptor = function () {
  var a = i18n.phonenumbers.PhoneNumberDesc.descriptor_;
  a || (i18n.phonenumbers.PhoneNumberDesc.descriptor_ = a = goog.proto2.Message.createDescriptor(i18n.phonenumbers.PhoneNumberDesc
, {0:{name:"PhoneNumberDesc", fullName:"i18n.phonenumbers.PhoneNumberDesc"}, 2:{name:"national_number_pattern", fieldType:goog.proto2
.Message.FieldType.STRING, type:String}, 3:{name:"possible_number_pattern", fieldType:goog.proto2.Message.FieldType.STRING, type
:String}, 9:{name:"possible_length", repeated:!0, fieldType:goog.proto2.Message.FieldType.INT32, type:Number},
  10:{name:"possible_length_local_only", repeated:!0, fieldType:goog.proto2.Message.FieldType.INT32, type:Number}, 6:{name:"example_number
", fieldType:goog.proto2.Message.FieldType.STRING, type:String}, 7:{name:"national_number_matcher_data", fieldType:goog.proto2.Message
.FieldType.BYTES, type:String}, 8:{name:"possible_number_matcher_data", fieldType:goog.proto2.Message.FieldType.BYTES, type:String
}}));
  return a;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.google-libphonenumber.PhoneNumberDesc.prototype"></a>[module google-libphonenumber.PhoneNumberDesc.prototype](#apidoc.module.google-libphonenumber.PhoneNumberDesc.prototype)

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.addPossibleLength"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>addPossibleLength (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.addPossibleLength)
- description and source-code
```javascript
addPossibleLength = function (a) {
  this.add$Value(9, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.addPossibleLengthLocalOnly"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>addPossibleLengthLocalOnly (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.addPossibleLengthLocalOnly)
- description and source-code
```javascript
addPossibleLengthLocalOnly = function (a) {
  this.add$Value(10, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearExampleNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>clearExampleNumber ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearExampleNumber)
- description and source-code
```javascript
clearExampleNumber = function () {
  this.clear$Field(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearNationalNumberMatcherData"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>clearNationalNumberMatcherData ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearNationalNumberMatcherData)
- description and source-code
```javascript
clearNationalNumberMatcherData = function () {
  this.clear$Field(7);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearNationalNumberPattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>clearNationalNumberPattern ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearNationalNumberPattern)
- description and source-code
```javascript
clearNationalNumberPattern = function () {
  this.clear$Field(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearPossibleLength"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>clearPossibleLength ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearPossibleLength)
- description and source-code
```javascript
clearPossibleLength = function () {
  this.clear$Field(9);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearPossibleLengthLocalOnly"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>clearPossibleLengthLocalOnly ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearPossibleLengthLocalOnly)
- description and source-code
```javascript
clearPossibleLengthLocalOnly = function () {
  this.clear$Field(10);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearPossibleNumberMatcherData"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>clearPossibleNumberMatcherData ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearPossibleNumberMatcherData)
- description and source-code
```javascript
clearPossibleNumberMatcherData = function () {
  this.clear$Field(8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearPossibleNumberPattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>clearPossibleNumberPattern ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.clearPossibleNumberPattern)
- description and source-code
```javascript
clearPossibleNumberPattern = function () {
  this.clear$Field(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.constructor"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>constructor ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
  goog.proto2.Message.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.exampleNumberCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>exampleNumberCount ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.exampleNumberCount)
- description and source-code
```javascript
exampleNumberCount = function () {
  return this.count$Values(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getDescriptor"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getDescriptor ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getDescriptor)
- description and source-code
```javascript
getDescriptor = function () {
  var a = i18n.phonenumbers.PhoneNumberDesc.descriptor_;
  a || (i18n.phonenumbers.PhoneNumberDesc.descriptor_ = a = goog.proto2.Message.createDescriptor(i18n.phonenumbers.PhoneNumberDesc
, {0:{name:"PhoneNumberDesc", fullName:"i18n.phonenumbers.PhoneNumberDesc"}, 2:{name:"national_number_pattern", fieldType:goog.proto2
.Message.FieldType.STRING, type:String}, 3:{name:"possible_number_pattern", fieldType:goog.proto2.Message.FieldType.STRING, type
:String}, 9:{name:"possible_length", repeated:!0, fieldType:goog.proto2.Message.FieldType.INT32, type:Number},
  10:{name:"possible_length_local_only", repeated:!0, fieldType:goog.proto2.Message.FieldType.INT32, type:Number}, 6:{name:"example_number
", fieldType:goog.proto2.Message.FieldType.STRING, type:String}, 7:{name:"national_number_matcher_data", fieldType:goog.proto2.Message
.FieldType.BYTES, type:String}, 8:{name:"possible_number_matcher_data", fieldType:goog.proto2.Message.FieldType.BYTES, type:String
}}));
  return a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getExampleNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getExampleNumber ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getExampleNumber)
- description and source-code
```javascript
getExampleNumber = function () {
  return this.get$Value(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getExampleNumberOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getExampleNumberOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getExampleNumberOrDefault)
- description and source-code
```javascript
getExampleNumberOrDefault = function () {
  return this.get$ValueOrDefault(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getNationalNumberMatcherData"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getNationalNumberMatcherData ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getNationalNumberMatcherData)
- description and source-code
```javascript
getNationalNumberMatcherData = function () {
  return this.get$Value(7);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getNationalNumberMatcherDataOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getNationalNumberMatcherDataOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getNationalNumberMatcherDataOrDefault)
- description and source-code
```javascript
getNationalNumberMatcherDataOrDefault = function () {
  return this.get$ValueOrDefault(7);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getNationalNumberPattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getNationalNumberPattern ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getNationalNumberPattern)
- description and source-code
```javascript
getNationalNumberPattern = function () {
  return this.get$Value(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getNationalNumberPatternOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getNationalNumberPatternOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getNationalNumberPatternOrDefault)
- description and source-code
```javascript
getNationalNumberPatternOrDefault = function () {
  return this.get$ValueOrDefault(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleLength"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getPossibleLength (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleLength)
- description and source-code
```javascript
getPossibleLength = function (a) {
  return this.get$Value(9, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleLengthLocalOnly"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getPossibleLengthLocalOnly (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleLengthLocalOnly)
- description and source-code
```javascript
getPossibleLengthLocalOnly = function (a) {
  return this.get$Value(10, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleLengthLocalOnlyOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getPossibleLengthLocalOnlyOrDefault (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleLengthLocalOnlyOrDefault)
- description and source-code
```javascript
getPossibleLengthLocalOnlyOrDefault = function (a) {
  return this.get$ValueOrDefault(10, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleLengthOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getPossibleLengthOrDefault (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleLengthOrDefault)
- description and source-code
```javascript
getPossibleLengthOrDefault = function (a) {
  return this.get$ValueOrDefault(9, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleNumberMatcherData"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getPossibleNumberMatcherData ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleNumberMatcherData)
- description and source-code
```javascript
getPossibleNumberMatcherData = function () {
  return this.get$Value(8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleNumberMatcherDataOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getPossibleNumberMatcherDataOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleNumberMatcherDataOrDefault)
- description and source-code
```javascript
getPossibleNumberMatcherDataOrDefault = function () {
  return this.get$ValueOrDefault(8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleNumberPattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getPossibleNumberPattern ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleNumberPattern)
- description and source-code
```javascript
getPossibleNumberPattern = function () {
  return this.get$Value(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleNumberPatternOrDefault"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>getPossibleNumberPatternOrDefault ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.getPossibleNumberPatternOrDefault)
- description and source-code
```javascript
getPossibleNumberPatternOrDefault = function () {
  return this.get$ValueOrDefault(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasExampleNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>hasExampleNumber ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasExampleNumber)
- description and source-code
```javascript
hasExampleNumber = function () {
  return this.has$Value(6);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasNationalNumberMatcherData"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>hasNationalNumberMatcherData ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasNationalNumberMatcherData)
- description and source-code
```javascript
hasNationalNumberMatcherData = function () {
  return this.has$Value(7);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasNationalNumberPattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>hasNationalNumberPattern ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasNationalNumberPattern)
- description and source-code
```javascript
hasNationalNumberPattern = function () {
  return this.has$Value(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasPossibleLength"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>hasPossibleLength ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasPossibleLength)
- description and source-code
```javascript
hasPossibleLength = function () {
  return this.has$Value(9);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasPossibleLengthLocalOnly"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>hasPossibleLengthLocalOnly ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasPossibleLengthLocalOnly)
- description and source-code
```javascript
hasPossibleLengthLocalOnly = function () {
  return this.has$Value(10);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasPossibleNumberMatcherData"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>hasPossibleNumberMatcherData ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasPossibleNumberMatcherData)
- description and source-code
```javascript
hasPossibleNumberMatcherData = function () {
  return this.has$Value(8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasPossibleNumberPattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>hasPossibleNumberPattern ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.hasPossibleNumberPattern)
- description and source-code
```javascript
hasPossibleNumberPattern = function () {
  return this.has$Value(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.nationalNumberMatcherDataCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>nationalNumberMatcherDataCount ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.nationalNumberMatcherDataCount)
- description and source-code
```javascript
nationalNumberMatcherDataCount = function () {
  return this.count$Values(7);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.nationalNumberPatternCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>nationalNumberPatternCount ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.nationalNumberPatternCount)
- description and source-code
```javascript
nationalNumberPatternCount = function () {
  return this.count$Values(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.possibleLengthArray"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>possibleLengthArray ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.possibleLengthArray)
- description and source-code
```javascript
possibleLengthArray = function () {
  return this.array$Values(9);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.possibleLengthCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>possibleLengthCount ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.possibleLengthCount)
- description and source-code
```javascript
possibleLengthCount = function () {
  return this.count$Values(9);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.possibleLengthLocalOnlyArray"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>possibleLengthLocalOnlyArray ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.possibleLengthLocalOnlyArray)
- description and source-code
```javascript
possibleLengthLocalOnlyArray = function () {
  return this.array$Values(10);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.possibleLengthLocalOnlyCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>possibleLengthLocalOnlyCount ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.possibleLengthLocalOnlyCount)
- description and source-code
```javascript
possibleLengthLocalOnlyCount = function () {
  return this.count$Values(10);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.possibleNumberMatcherDataCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>possibleNumberMatcherDataCount ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.possibleNumberMatcherDataCount)
- description and source-code
```javascript
possibleNumberMatcherDataCount = function () {
  return this.count$Values(8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.possibleNumberPatternCount"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>possibleNumberPatternCount ()](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.possibleNumberPatternCount)
- description and source-code
```javascript
possibleNumberPatternCount = function () {
  return this.count$Values(3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.setExampleNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>setExampleNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.setExampleNumber)
- description and source-code
```javascript
setExampleNumber = function (a) {
  this.set$Value(6, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.setNationalNumberMatcherData"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>setNationalNumberMatcherData (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.setNationalNumberMatcherData)
- description and source-code
```javascript
setNationalNumberMatcherData = function (a) {
  this.set$Value(7, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.setNationalNumberPattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>setNationalNumberPattern (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.setNationalNumberPattern)
- description and source-code
```javascript
setNationalNumberPattern = function (a) {
  this.set$Value(2, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.setPossibleNumberMatcherData"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>setPossibleNumberMatcherData (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.setPossibleNumberMatcherData)
- description and source-code
```javascript
setPossibleNumberMatcherData = function (a) {
  this.set$Value(8, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.setPossibleNumberPattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberDesc.prototype.</span>setPossibleNumberPattern (a)](#apidoc.element.google-libphonenumber.PhoneNumberDesc.prototype.setPossibleNumberPattern)
- description and source-code
```javascript
setPossibleNumberPattern = function (a) {
  this.set$Value(3, a);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.google-libphonenumber.PhoneNumberUtil"></a>[module google-libphonenumber.PhoneNumberUtil](#apidoc.module.google-libphonenumber.PhoneNumberUtil)

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.PhoneNumberUtil"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.</span>PhoneNumberUtil ()](#apidoc.element.google-libphonenumber.PhoneNumberUtil.PhoneNumberUtil)
- description and source-code
```javascript
PhoneNumberUtil = function () {
  this.regionToMetadataMap = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.convertAlphaCharactersInNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>convertAlphaCharactersInNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.convertAlphaCharactersInNumber)
- description and source-code
```javascript
convertAlphaCharactersInNumber = function (a) {
  return i18n.phonenumbers.PhoneNumberUtil.normalizeHelper_(a, i18n.phonenumbers.PhoneNumberUtil.ALL_NORMALIZATION_MAPPINGS_, !1
);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.copyCoreFieldsOnly_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>copyCoreFieldsOnly_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.copyCoreFieldsOnly_)
- description and source-code
```javascript
copyCoreFieldsOnly_ = function (a) {
  var b = new i18n.phonenumbers.PhoneNumber;
  b.setCountryCode(a.getCountryCodeOrDefault());
  b.setNationalNumber(a.getNationalNumberOrDefault());
  0 < a.getExtensionOrDefault().length && b.setExtension(a.getExtensionOrDefault());
  a.getItalianLeadingZero() && (b.setItalianLeadingZero(!0), b.setNumberOfLeadingZeros(a.getNumberOfLeadingZerosOrDefault()));
  return b;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.descHasData_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>descHasData_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.descHasData_)
- description and source-code
```javascript
descHasData_ = function (a) {
  return null != a && (a.hasExampleNumber() || i18n.phonenumbers.PhoneNumberUtil.descHasPossibleNumberData_(a) || a.hasNationalNumberPattern
 && "NA" != a.getNationalNumberPatternOrDefault());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.descHasPossibleNumberData_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>descHasPossibleNumberData_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.descHasPossibleNumberData_)
- description and source-code
```javascript
descHasPossibleNumberData_ = function (a) {
  return null != a && (1 != a.possibleLengthCount() || -1 != a.possibleLengthArray()[0]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.extractPossibleNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>extractPossibleNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.extractPossibleNumber)
- description and source-code
```javascript
extractPossibleNumber = function (a) {
  var b = a.search(i18n.phonenumbers.PhoneNumberUtil.VALID_START_CHAR_PATTERN_);
  0 <= b ? (a = a.substring(b), a = a.replace(i18n.phonenumbers.PhoneNumberUtil.UNWANTED_END_CHAR_PATTERN_, ""), b = a.search(i18n
.phonenumbers.PhoneNumberUtil.SECOND_NUMBER_START_PATTERN_), 0 <= b && (a = a.substring(0, b))) : a = "";
  return a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.getCountryMobileToken"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>getCountryMobileToken (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.getCountryMobileToken)
- description and source-code
```javascript
getCountryMobileToken = function (a) {
  return i18n.phonenumbers.PhoneNumberUtil.MOBILE_TOKEN_MAPPINGS_[a] || "";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.getInstance"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>getInstance ()](#apidoc.element.google-libphonenumber.PhoneNumberUtil.getInstance)
- description and source-code
```javascript
getInstance = function () {
  if (a.instance_) {
    return a.instance_;
  }
  goog.DEBUG && (goog.instantiatedSingletons_[goog.instantiatedSingletons_.length] = a);
  return a.instance_ = new a;
}
```
- example usage
```shell
...
Here's a simple example on how to format a US-based number in the international phone number format:

'''js
// Require 'PhoneNumberFormat'.
var PNF = require('google-libphonenumber').PhoneNumberFormat;

// Get an instance of 'PhoneNumberUtil'.
var phoneUtil = require('google-libphonenumber').PhoneNumberUtil.getInstance();

// Parse number with country code.
var phoneNumber = phoneUtil.parse('202-456-1414', 'US');

// Print number in the international format.
console.log(phoneUtil.format(phoneNumber, PNF.INTERNATIONAL));
// => +1 202-456-1414
...
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.getNumberDescByType_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>getNumberDescByType_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.getNumberDescByType_)
- description and source-code
```javascript
getNumberDescByType_ = function (a, b) {
  switch(b) {
    case i18n.phonenumbers.PhoneNumberType.PREMIUM_RATE:
      return a.getPremiumRate();
    case i18n.phonenumbers.PhoneNumberType.TOLL_FREE:
      return a.getTollFree();
    case i18n.phonenumbers.PhoneNumberType.MOBILE:
      return a.getMobile();
    case i18n.phonenumbers.PhoneNumberType.FIXED_LINE:
    case i18n.phonenumbers.PhoneNumberType.FIXED_LINE_OR_MOBILE:
      return a.getFixedLine();
    case i18n.phonenumbers.PhoneNumberType.SHARED_COST:
      return a.getSharedCost();
    case i18n.phonenumbers.PhoneNumberType.VOIP:
      return a.getVoip();
    case i18n.phonenumbers.PhoneNumberType.PERSONAL_NUMBER:
      return a.getPersonalNumber();
    case i18n.phonenumbers.PhoneNumberType.PAGER:
      return a.getPager();
    case i18n.phonenumbers.PhoneNumberType.UAN:
      return a.getUan();
    case i18n.phonenumbers.PhoneNumberType.VOICEMAIL:
      return a.getVoicemail();
    default:
      return a.getGeneralDesc();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.getSupportedTypesForMetadata_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>getSupportedTypesForMetadata_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.getSupportedTypesForMetadata_)
- description and source-code
```javascript
getSupportedTypesForMetadata_ = function (a) {
  var b = [];
  goog.object.forEach(i18n.phonenumbers.PhoneNumberType, function(c) {
    if (c != i18n.phonenumbers.PhoneNumberType.FIXED_LINE_OR_MOBILE && c != i18n.phonenumbers.PhoneNumberType.UNKNOWN) {
      var d = i18n.phonenumbers.PhoneNumberUtil.getNumberDescByType_(a, c);
      i18n.phonenumbers.PhoneNumberUtil.descHasData_(d) && b.push(c);
    }
  });
  return b;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.isViablePhoneNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>isViablePhoneNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.isViablePhoneNumber)
- description and source-code
```javascript
isViablePhoneNumber = function (a) {
  return a.length < i18n.phonenumbers.PhoneNumberUtil.MIN_LENGTH_FOR_NSN_ ? !1 : i18n.phonenumbers.PhoneNumberUtil.matchesEntirely_
(i18n.phonenumbers.PhoneNumberUtil.VALID_PHONE_NUMBER_PATTERN_, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.matchesEntirely_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>matchesEntirely_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.matchesEntirely_)
- description and source-code
```javascript
matchesEntirely_ = function (a, b) {
  var c = "string" == typeof a ? b.match("^(?:" + a + ")$") : b.match(a);
  return c && c[0].length == b.length ? !0 : !1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.normalize"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>normalize (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.normalize)
- description and source-code
```javascript
normalize = function (a) {
  return i18n.phonenumbers.PhoneNumberUtil.matchesEntirely_(i18n.phonenumbers.PhoneNumberUtil.VALID_ALPHA_PHONE_PATTERN_, a) ? i18n
.phonenumbers.PhoneNumberUtil.normalizeHelper_(a, i18n.phonenumbers.PhoneNumberUtil.ALL_NORMALIZATION_MAPPINGS_, !0) : i18n.phonenumbers
.PhoneNumberUtil.normalizeDigitsOnly(a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.normalizeDiallableCharsOnly"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>normalizeDiallableCharsOnly (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.normalizeDiallableCharsOnly)
- description and source-code
```javascript
normalizeDiallableCharsOnly = function (a) {
  return i18n.phonenumbers.PhoneNumberUtil.normalizeHelper_(a, i18n.phonenumbers.PhoneNumberUtil.DIALLABLE_CHAR_MAPPINGS_, !0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.normalizeDigitsOnly"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>normalizeDigitsOnly (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.normalizeDigitsOnly)
- description and source-code
```javascript
normalizeDigitsOnly = function (a) {
  return i18n.phonenumbers.PhoneNumberUtil.normalizeHelper_(a, i18n.phonenumbers.PhoneNumberUtil.DIGIT_MAPPINGS, !0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.normalizeHelper_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>normalizeHelper_ (a, b, c)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.normalizeHelper_)
- description and source-code
```javascript
normalizeHelper_ = function (a, b, c) {
  for (var d = new goog.string.StringBuffer, e, f, g = a.length, h = 0;h < g;++h) {
    e = a.charAt(h), f = b[e.toUpperCase()], null != f ? d.append(f) : c || d.append(e);
  }
  return d.toString();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.normalizeSB_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>normalizeSB_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.normalizeSB_)
- description and source-code
```javascript
normalizeSB_ = function (a) {
  var b = i18n.phonenumbers.PhoneNumberUtil.normalize(a.toString());
  a.clear();
  a.append(b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.setItalianLeadingZerosForPhoneNumber_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.</span>setItalianLeadingZerosForPhoneNumber_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.setItalianLeadingZerosForPhoneNumber_)
- description and source-code
```javascript
setItalianLeadingZerosForPhoneNumber_ = function (a, b) {
  if (1 < a.length && "0" == a.charAt(0)) {
    b.setItalianLeadingZero(!0);
    for (var c = 1;c < a.length - 1 && "0" == a.charAt(c);) {
      c++;
    }
    1 != c && b.setNumberOfLeadingZeros(c);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.google-libphonenumber.PhoneNumberUtil.prototype"></a>[module google-libphonenumber.PhoneNumberUtil.prototype](#apidoc.module.google-libphonenumber.PhoneNumberUtil.prototype)

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.buildNationalNumberForParsing_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>buildNationalNumberForParsing_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.buildNationalNumberForParsing_)
- description and source-code
```javascript
buildNationalNumberForParsing_ = function (a, b) {
  var c = a.indexOf(i18n.phonenumbers.PhoneNumberUtil.RFC3966_PHONE_CONTEXT_);
  if (0 < c) {
    var d = c + i18n.phonenumbers.PhoneNumberUtil.RFC3966_PHONE_CONTEXT_.length;
    if (a.charAt(d) == i18n.phonenumbers.PhoneNumberUtil.PLUS_SIGN) {
      var e = a.indexOf(";", d);
      0 < e ? b.append(a.substring(d, e)) : b.append(a.substring(d));
    }
    d = a.indexOf(i18n.phonenumbers.PhoneNumberUtil.RFC3966_PREFIX_);
    b.append(a.substring(0 <= d ? d + i18n.phonenumbers.PhoneNumberUtil.RFC3966_PREFIX_.length : 0, c));
  } else {
    b.append(i18n.phonenumbers.PhoneNumberUtil.extractPossibleNumber(a));
  }
  c = b.toString();
  d = c.indexOf(i18n.phonenumbers.PhoneNumberUtil.RFC3966_ISDN_SUBADDRESS_);
  0 < d && (b.clear(), b.append(c.substring(0, d)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.canBeInternationallyDialled"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>canBeInternationallyDialled (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.canBeInternationallyDialled)
- description and source-code
```javascript
canBeInternationallyDialled = function (a) {
  var b = this.getMetadataForRegion(this.getRegionCodeForNumber(a));
  if (null == b) {
    return !0;
  }
  a = this.getNationalSignificantNumber(a);
  return !this.isNumberMatchingDesc_(a, b.getNoInternationalDialling());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.checkRegionForParsing_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>checkRegionForParsing_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.checkRegionForParsing_)
- description and source-code
```javascript
checkRegionForParsing_ = function (a, b) {
  return this.isValidRegionCode_(b) || null != a && 0 < a.length && i18n.phonenumbers.PhoneNumberUtil.LEADING_PLUS_CHARS_PATTERN_
.test(a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.chooseFormattingPatternForNumber_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>chooseFormattingPatternForNumber_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.chooseFormattingPatternForNumber_)
- description and source-code
```javascript
chooseFormattingPatternForNumber_ = function (a, b) {
  for (var c, d = a.length, e = 0;e < d;++e) {
    c = a[e];
    var f = c.leadingDigitsPatternCount();
    if (0 == f || 0 == b.search(c.getLeadingDigitsPattern(f - 1))) {
      if (f = new RegExp(c.getPattern()), i18n.phonenumbers.PhoneNumberUtil.matchesEntirely_(f, b)) {
        return c;
      }
    }
  }
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.extractCountryCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>extractCountryCode (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.extractCountryCode)
- description and source-code
```javascript
extractCountryCode = function (a, b) {
  var c = a.toString();
  if (0 == c.length || "0" == c.charAt(0)) {
    return 0;
  }
  for (var d, e = c.length, f = 1;f <= i18n.phonenumbers.PhoneNumberUtil.MAX_LENGTH_COUNTRY_CODE_ && f <= e;++f) {
    if (d = parseInt(c.substring(0, f), 10), d in i18n.phonenumbers.metadata.countryCodeToRegionCodeMap) {
      return b.append(c.substring(f)), d;
    }
  }
  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.format"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>format (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.format)
- description and source-code
```javascript
format = function (a, b) {
  if (0 == a.getNationalNumber() && a.hasRawInput()) {
    var c = a.getRawInputOrDefault();
    if (0 < c.length) {
      return c;
    }
  }
  var c = a.getCountryCodeOrDefault(), d = this.getNationalSignificantNumber(a);
  if (b == i18n.phonenumbers.PhoneNumberFormat.E164) {
    return this.prefixNumberWithCountryCallingCode_(c, i18n.phonenumbers.PhoneNumberFormat.E164, d, "");
  }
  if (!this.hasValidCountryCallingCode_(c)) {
    return d;
  }
  var e = this.getRegionCodeForCountryCode(c), f = this.getMetadataForRegionOrCallingCode_(c, e), e = this.maybeGetFormattedExtension_
(a, f, b), d = this.formatNsn_(d, f, b);
  return this.prefixNumberWithCountryCallingCode_(c, b, d, e);
}
```
- example usage
```shell
...
// Get an instance of 'PhoneNumberUtil'.
var phoneUtil = require('google-libphonenumber').PhoneNumberUtil.getInstance();

// Parse number with country code.
var phoneNumber = phoneUtil.parse('202-456-1414', 'US');

// Print number in the international format.
console.log(phoneUtil.format(phoneNumber, PNF.INTERNATIONAL));
// => +1 202-456-1414
'''

#### Using the "As You Type" Formatter

'''js
// Require 'AsYouTypeFormatter'.
...
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatByPattern"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formatByPattern (a, b, c)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatByPattern)
- description and source-code
```javascript
formatByPattern = function (a, b, c) {
  var d = a.getCountryCodeOrDefault(), e = this.getNationalSignificantNumber(a);
  if (!this.hasValidCountryCallingCode_(d)) {
    return e;
  }
  var f = this.getRegionCodeForCountryCode(d), f = this.getMetadataForRegionOrCallingCode_(d, f), g = this.chooseFormattingPatternForNumber_
(c, e);
  if (null != g) {
    c = g.clone();
    g = g.getNationalPrefixFormattingRuleOrDefault();
    if (0 < g.length) {
      var h = f.getNationalPrefixOrDefault();
      0 < h.length ? (g = g.replace(i18n.phonenumbers.PhoneNumberUtil.NP_PATTERN_, h).replace(i18n.phonenumbers.PhoneNumberUtil.
FG_PATTERN_, "$1"), c.setNationalPrefixFormattingRule(g)) : c.clearNationalPrefixFormattingRule();
    }
    e = this.formatNsnUsingPattern_(e, c, b);
  }
  a = this.maybeGetFormattedExtension_(a, f, b);
  return this.prefixNumberWithCountryCallingCode_(d, b, e, a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatInOriginalFormat"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formatInOriginalFormat (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatInOriginalFormat)
- description and source-code
```javascript
formatInOriginalFormat = function (a, b) {
  if (a.hasRawInput() && (this.hasUnexpectedItalianLeadingZero_(a) || !this.hasFormattingPatternForNumber_(a))) {
    return a.getRawInputOrDefault();
  }
  if (!a.hasCountryCodeSource()) {
    return this.format(a, i18n.phonenumbers.PhoneNumberFormat.NATIONAL);
  }
  var c;
  switch(a.getCountryCodeSource()) {
    case i18n.phonenumbers.PhoneNumber.CountryCodeSource.FROM_NUMBER_WITH_PLUS_SIGN:
      c = this.format(a, i18n.phonenumbers.PhoneNumberFormat.INTERNATIONAL);
      break;
    case i18n.phonenumbers.PhoneNumber.CountryCodeSource.FROM_NUMBER_WITH_IDD:
      c = this.formatOutOfCountryCallingNumber(a, b);
      break;
    case i18n.phonenumbers.PhoneNumber.CountryCodeSource.FROM_NUMBER_WITHOUT_PLUS_SIGN:
      c = this.format(a, i18n.phonenumbers.PhoneNumberFormat.INTERNATIONAL).substring(1);
      break;
    default:
      var d = this.getRegionCodeForCountryCode(a.getCountryCodeOrDefault()), e = this.getNddPrefixForRegion(d, !0);
      c = this.format(a, i18n.phonenumbers.PhoneNumberFormat.NATIONAL);
      if (null != e && 0 != e.length && !this.rawInputContainsNationalPrefix_(a.getRawInputOrDefault(), e, d) && (d = this.getMetadataForRegion
(d), e = this.getNationalSignificantNumber(a), d = this.chooseFormattingPatternForNumber_(d.numberFormatArray(), e), null != d)) {
        var e = d.getNationalPrefixFormattingRuleOrDefault(), f = e.indexOf("$1");
        0 >= f || (e = e.substring(0, f), e = i18n.phonenumbers.PhoneNumberUtil.normalizeDigitsOnly(e), 0 != e.length && (c = d.
clone(), c.clearNationalPrefixFormattingRule(), c = this.formatByPattern(a, i18n.phonenumbers.PhoneNumberFormat.NATIONAL, [c])));
      }
  }
  d = a.getRawInputOrDefault();
  null != c && 0 < d.length && (e = i18n.phonenumbers.PhoneNumberUtil.normalizeDiallableCharsOnly(c), f = i18n.phonenumbers.PhoneNumberUtil
.normalizeDiallableCharsOnly(d), e != f && (c = d));
  return c;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatNationalNumberWithCarrierCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formatNationalNumberWithCarrierCode (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatNationalNumberWithCarrierCode)
- description and source-code
```javascript
formatNationalNumberWithCarrierCode = function (a, b) {
  var c = a.getCountryCodeOrDefault(), d = this.getNationalSignificantNumber(a);
  if (!this.hasValidCountryCallingCode_(c)) {
    return d;
  }
  var e = this.getRegionCodeForCountryCode(c), f = this.getMetadataForRegionOrCallingCode_(c, e), e = this.maybeGetFormattedExtension_
(a, f, i18n.phonenumbers.PhoneNumberFormat.NATIONAL), d = this.formatNsn_(d, f, i18n.phonenumbers.PhoneNumberFormat.NATIONAL, b);
  return this.prefixNumberWithCountryCallingCode_(c, i18n.phonenumbers.PhoneNumberFormat.NATIONAL, d, e);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatNationalNumberWithPreferredCarrierCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formatNationalNumberWithPreferredCarrierCode (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatNationalNumberWithPreferredCarrierCode)
- description and source-code
```javascript
formatNationalNumberWithPreferredCarrierCode = function (a, b) {
  return this.formatNationalNumberWithCarrierCode(a, 0 < a.getPreferredDomesticCarrierCodeOrDefault().length ? a.getPreferredDomesticCarrierCodeOrDefault
() : b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatNsnUsingPattern_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formatNsnUsingPattern_ (a, b, c, d)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatNsnUsingPattern_)
- description and source-code
```javascript
formatNsnUsingPattern_ = function (a, b, c, d) {
  var e = b.getFormatOrDefault(), f = new RegExp(b.getPattern()), g = b.getDomesticCarrierCodeFormattingRuleOrDefault();
  c == i18n.phonenumbers.PhoneNumberFormat.NATIONAL && null != d && 0 < d.length && 0 < g.length ? (b = g.replace(i18n.phonenumbers
.PhoneNumberUtil.CC_PATTERN_, d), e = e.replace(i18n.phonenumbers.PhoneNumberUtil.FIRST_GROUP_PATTERN_, b), a = a.replace(f, e)) : (
b = b.getNationalPrefixFormattingRuleOrDefault(), a = c == i18n.phonenumbers.PhoneNumberFormat.NATIONAL && null != b && 0 < b.length
 ? a.replace(f, e.replace(i18n.phonenumbers.PhoneNumberUtil.FIRST_GROUP_PATTERN_, b)) : a.replace(f, e));
  c == i18n.phonenumbers.PhoneNumberFormat.RFC3966 && (a = a.replace(new RegExp("^" + i18n.phonenumbers.PhoneNumberUtil.SEPARATOR_PATTERN_
), ""), a = a.replace(new RegExp(i18n.phonenumbers.PhoneNumberUtil.SEPARATOR_PATTERN_, "g"), "-"));
  return a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatNsn_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formatNsn_ (a, b, c, d)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatNsn_)
- description and source-code
```javascript
formatNsn_ = function (a, b, c, d) {
  b = 0 == b.intlNumberFormatArray().length || c == i18n.phonenumbers.PhoneNumberFormat.NATIONAL ? b.numberFormatArray() : b.intlNumberFormatArray
();
  b = this.chooseFormattingPatternForNumber_(b, a);
  return null == b ? a : this.formatNsnUsingPattern_(a, b, c, d);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatNumberForMobileDialing"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formatNumberForMobileDialing (a, b, c)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatNumberForMobileDialing)
- description and source-code
```javascript
formatNumberForMobileDialing = function (a, b, c) {
  var d = a.getCountryCodeOrDefault();
  if (!this.hasValidCountryCallingCode_(d)) {
    return a.hasRawInput() ? a.getRawInputOrDefault() : "";
  }
  var e = "";
  a = a.clone();
  a.clearExtension();
  var f = this.getRegionCodeForCountryCode(d), g = this.getNumberType(a), h = g != i18n.phonenumbers.PhoneNumberType.UNKNOWN;
  if (b == f) {
    e = g == i18n.phonenumbers.PhoneNumberType.FIXED_LINE || g == i18n.phonenumbers.PhoneNumberType.MOBILE || g == i18n.phonenumbers
.PhoneNumberType.FIXED_LINE_OR_MOBILE, "CO" == f && g == i18n.phonenumbers.PhoneNumberType.FIXED_LINE ? e = this.formatNationalNumberWithCarrierCode
(a, i18n.phonenumbers.PhoneNumberUtil.COLOMBIA_MOBILE_TO_FIXED_LINE_PREFIX_) : "BR" == f && e ? e = 0 < a.getPreferredDomesticCarrierCodeOrDefault
().length ? this.formatNationalNumberWithPreferredCarrierCode(a, "") : "" :
    h && "HU" == f ? e = this.getNddPrefixForRegion(f, !0) + " " + this.format(a, i18n.phonenumbers.PhoneNumberFormat.NATIONAL) :
d == i18n.phonenumbers.PhoneNumberUtil.NANPA_COUNTRY_CODE_ ? (b = this.getMetadataForRegion(b), e = this.canBeInternationallyDialled
(a) && this.testNumberLength_(this.getNationalSignificantNumber(a), b) != i18n.phonenumbers.PhoneNumberUtil.ValidationResult.TOO_SHORT
 ? this.format(a, i18n.phonenumbers.PhoneNumberFormat.INTERNATIONAL) : this.format(a, i18n.phonenumbers.PhoneNumberFormat.NATIONAL
)) :
    e = (f == i18n.phonenumbers.PhoneNumberUtil.REGION_CODE_FOR_NON_GEO_ENTITY || ("MX" == f || "CL" == f) && e) && this.canBeInternationallyDialled
(a) ? this.format(a, i18n.phonenumbers.PhoneNumberFormat.INTERNATIONAL) : this.format(a, i18n.phonenumbers.PhoneNumberFormat.NATIONAL
);
  } else {
    if (h && this.canBeInternationallyDialled(a)) {
      return c ? this.format(a, i18n.phonenumbers.PhoneNumberFormat.INTERNATIONAL) : this.format(a, i18n.phonenumbers.PhoneNumberFormat
.E164);
    }
  }
  return c ? e : i18n.phonenumbers.PhoneNumberUtil.normalizeDiallableCharsOnly(e);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatOutOfCountryCallingNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formatOutOfCountryCallingNumber (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatOutOfCountryCallingNumber)
- description and source-code
```javascript
formatOutOfCountryCallingNumber = function (a, b) {
  if (!this.isValidRegionCode_(b)) {
    return this.format(a, i18n.phonenumbers.PhoneNumberFormat.INTERNATIONAL);
  }
  var c = a.getCountryCodeOrDefault(), d = this.getNationalSignificantNumber(a);
  if (!this.hasValidCountryCallingCode_(c)) {
    return d;
  }
  if (c == i18n.phonenumbers.PhoneNumberUtil.NANPA_COUNTRY_CODE_) {
    if (this.isNANPACountry(b)) {
      return c + " " + this.format(a, i18n.phonenumbers.PhoneNumberFormat.NATIONAL);
    }
  } else {
    if (c == this.getCountryCodeForValidRegion_(b)) {
      return this.format(a, i18n.phonenumbers.PhoneNumberFormat.NATIONAL);
    }
  }
  var e = this.getMetadataForRegion(b), f = e.getInternationalPrefixOrDefault(), g = "";
  i18n.phonenumbers.PhoneNumberUtil.matchesEntirely_(i18n.phonenumbers.PhoneNumberUtil.UNIQUE_INTERNATIONAL_PREFIX_, f) ? g = f :
e.hasPreferredInternationalPrefix() && (g = e.getPreferredInternationalPrefixOrDefault());
  e = this.getRegionCodeForCountryCode(c);
  e = this.getMetadataForRegionOrCallingCode_(c, e);
  d = this.formatNsn_(d, e, i18n.phonenumbers.PhoneNumberFormat.INTERNATIONAL);
  e = this.maybeGetFormattedExtension_(a, e, i18n.phonenumbers.PhoneNumberFormat.INTERNATIONAL);
  return 0 < g.length ? g + " " + c + " " + d + e : this.prefixNumberWithCountryCallingCode_(c, i18n.phonenumbers.PhoneNumberFormat
.INTERNATIONAL, d, e);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatOutOfCountryKeepingAlphaChars"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formatOutOfCountryKeepingAlphaChars (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formatOutOfCountryKeepingAlphaChars)
- description and source-code
```javascript
formatOutOfCountryKeepingAlphaChars = function (a, b) {
  var c = a.getRawInputOrDefault();
  if (0 == c.length) {
    return this.formatOutOfCountryCallingNumber(a, b);
  }
  var d = a.getCountryCodeOrDefault();
  if (!this.hasValidCountryCallingCode_(d)) {
    return c;
  }
  var c = i18n.phonenumbers.PhoneNumberUtil.normalizeHelper_(c, i18n.phonenumbers.PhoneNumberUtil.ALL_PLUS_NUMBER_GROUPING_SYMBOLS_
, !0), e = this.getNationalSignificantNumber(a);
  if (3 < e.length) {
    var f = c.indexOf(e.substring(0, 3));
    -1 != f && (c = c.substring(f));
  }
  f = this.getMetadataForRegion(b);
  if (d == i18n.phonenumbers.PhoneNumberUtil.NANPA_COUNTRY_CODE_) {
    if (this.isNANPACountry(b)) {
      return d + " " + c;
    }
  } else {
    if (null != f && d == this.getCountryCodeForValidRegion_(b)) {
      d = this.chooseFormattingPatternForNumber_(f.numberFormatArray(), e);
      if (null == d) {
        return c;
      }
      d = d.clone();
      d.setPattern("(\\d+)(.*)");
      d.setFormat("$1$2");
      return this.formatNsnUsingPattern_(c, d, i18n.phonenumbers.PhoneNumberFormat.NATIONAL);
    }
  }
  e = "";
  null != f && (e = f.getInternationalPrefixOrDefault(), e = i18n.phonenumbers.PhoneNumberUtil.matchesEntirely_(i18n.phonenumbers
.PhoneNumberUtil.UNIQUE_INTERNATIONAL_PREFIX_, e) ? e : f.getPreferredInternationalPrefixOrDefault());
  f = this.getRegionCodeForCountryCode(d);
  f = this.getMetadataForRegionOrCallingCode_(d, f);
  f = this.maybeGetFormattedExtension_(a, f, i18n.phonenumbers.PhoneNumberFormat.INTERNATIONAL);
  return 0 < e.length ? e + " " + d + " " + c + f : this.prefixNumberWithCountryCallingCode_(d, i18n.phonenumbers.PhoneNumberFormat
.INTERNATIONAL, c, f);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formattingRuleHasFirstGroupOnly"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>formattingRuleHasFirstGroupOnly (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.formattingRuleHasFirstGroupOnly)
- description and source-code
```javascript
formattingRuleHasFirstGroupOnly = function (a) {
  return 0 == a.length || i18n.phonenumbers.PhoneNumberUtil.FIRST_GROUP_ONLY_PREFIX_PATTERN_.test(a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getCountryCodeForRegion"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getCountryCodeForRegion (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getCountryCodeForRegion)
- description and source-code
```javascript
getCountryCodeForRegion = function (a) {
  return this.isValidRegionCode_(a) ? this.getCountryCodeForValidRegion_(a) : 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getCountryCodeForValidRegion_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getCountryCodeForValidRegion_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getCountryCodeForValidRegion_)
- description and source-code
```javascript
getCountryCodeForValidRegion_ = function (a) {
  var b = this.getMetadataForRegion(a);
  if (null == b) {
    throw Error("Invalid region code: " + a);
  }
  return b.getCountryCodeOrDefault();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getExampleNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getExampleNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getExampleNumber)
- description and source-code
```javascript
getExampleNumber = function (a) {
  return this.getExampleNumberForType(a, i18n.phonenumbers.PhoneNumberType.FIXED_LINE);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getExampleNumberForNonGeoEntity"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getExampleNumberForNonGeoEntity (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getExampleNumberForNonGeoEntity)
- description and source-code
```javascript
getExampleNumberForNonGeoEntity = function (a) {
  var b = this.getMetadataForNonGeographicalRegion(a);
  if (null != b && (b = goog.array.find([b.getMobile(), b.getTollFree(), b.getSharedCost(), b.getVoip(), b.getVoicemail(), b.getUan
(), b.getPremiumRate()], function(a, b) {
    return a.hasExampleNumber();
  }), null != b)) {
    try {
      return this.parse("+" + a + b.getExampleNumber(), "ZZ");
    } catch (c) {
    }
  }
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getExampleNumberForType"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getExampleNumberForType (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getExampleNumberForType)
- description and source-code
```javascript
getExampleNumberForType = function (a, b) {
  if (!this.isValidRegionCode_(a)) {
    return null;
  }
  var c = i18n.phonenumbers.PhoneNumberUtil.getNumberDescByType_(this.getMetadataForRegion(a), b);
  try {
    if (c.hasExampleNumber()) {
      return this.parse(c.getExampleNumber(), a);
    }
  } catch (d) {
  }
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getLengthOfGeographicalAreaCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getLengthOfGeographicalAreaCode (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getLengthOfGeographicalAreaCode)
- description and source-code
```javascript
getLengthOfGeographicalAreaCode = function (a) {
  var b = this.getMetadataForRegion(this.getRegionCodeForNumber(a));
  return null != b && (b.hasNationalPrefix() || a.hasItalianLeadingZero()) && this.isNumberGeographical(a) ? this.getLengthOfNationalDestinationCode
(a) : 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getLengthOfNationalDestinationCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getLengthOfNationalDestinationCode (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getLengthOfNationalDestinationCode)
- description and source-code
```javascript
getLengthOfNationalDestinationCode = function (a) {
  var b;
  a.hasExtension() ? (b = a.clone(), b.clearExtension()) : b = a;
  b = this.format(b, i18n.phonenumbers.PhoneNumberFormat.INTERNATIONAL).split(i18n.phonenumbers.PhoneNumberUtil.NON_DIGITS_PATTERN_
);
  0 == b[0].length && b.shift();
  return 2 >= b.length ? 0 : this.getNumberType(a) == i18n.phonenumbers.PhoneNumberType.MOBILE && (a = i18n.phonenumbers.PhoneNumberUtil
.getCountryMobileToken(a.getCountryCodeOrDefault()), "" != a) ? b[2].length + a.length : b[1].length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getMetadataForNonGeographicalRegion"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getMetadataForNonGeographicalRegion (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getMetadataForNonGeographicalRegion)
- description and source-code
```javascript
getMetadataForNonGeographicalRegion = function (a) {
  return this.getMetadataForRegion("" + a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getMetadataForRegion"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getMetadataForRegion (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getMetadataForRegion)
- description and source-code
```javascript
getMetadataForRegion = function (a) {
  if (null == a) {
    return null;
  }
  a = a.toUpperCase();
  var b = this.regionToMetadataMap[a];
  if (null == b) {
    var b = new goog.proto2.PbLiteSerializer, c = i18n.phonenumbers.metadata.countryToMetadata[a];
    if (null == c) {
      return null;
    }
    b = b.deserialize(i18n.phonenumbers.PhoneMetadata.getDescriptor(), c);
    this.regionToMetadataMap[a] = b;
  }
  return b;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getMetadataForRegionOrCallingCode_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getMetadataForRegionOrCallingCode_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getMetadataForRegionOrCallingCode_)
- description and source-code
```javascript
getMetadataForRegionOrCallingCode_ = function (a, b) {
  return i18n.phonenumbers.PhoneNumberUtil.REGION_CODE_FOR_NON_GEO_ENTITY == b ? this.getMetadataForNonGeographicalRegion(a) : this
.getMetadataForRegion(b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getNationalSignificantNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getNationalSignificantNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getNationalSignificantNumber)
- description and source-code
```javascript
getNationalSignificantNumber = function (a) {
  var b = "" + a.getNationalNumber();
  return a.hasItalianLeadingZero() && a.getItalianLeadingZero() && 0 < a.getNumberOfLeadingZerosOrDefault() ? Array(a.getNumberOfLeadingZerosOrDefault
() + 1).join("0") + b : b;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getNddPrefixForRegion"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getNddPrefixForRegion (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getNddPrefixForRegion)
- description and source-code
```javascript
getNddPrefixForRegion = function (a, b) {
  var c = this.getMetadataForRegion(a);
  if (null == c) {
    return null;
  }
  c = c.getNationalPrefixOrDefault();
  if (0 == c.length) {
    return null;
  }
  b && (c = c.replace("~", ""));
  return c;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getNumberType"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getNumberType (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getNumberType)
- description and source-code
```javascript
getNumberType = function (a) {
  var b = this.getRegionCodeForNumber(a), b = this.getMetadataForRegionOrCallingCode_(a.getCountryCodeOrDefault(), b);
  if (null == b) {
    return i18n.phonenumbers.PhoneNumberType.UNKNOWN;
  }
  a = this.getNationalSignificantNumber(a);
  return this.getNumberTypeHelper_(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getNumberTypeHelper_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getNumberTypeHelper_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getNumberTypeHelper_)
- description and source-code
```javascript
getNumberTypeHelper_ = function (a, b) {
  return this.isNumberMatchingDesc_(a, b.getGeneralDesc()) ? this.isNumberMatchingDesc_(a, b.getPremiumRate()) ? i18n.phonenumbers
.PhoneNumberType.PREMIUM_RATE : this.isNumberMatchingDesc_(a, b.getTollFree()) ? i18n.phonenumbers.PhoneNumberType.TOLL_FREE : this
.isNumberMatchingDesc_(a, b.getSharedCost()) ? i18n.phonenumbers.PhoneNumberType.SHARED_COST : this.isNumberMatchingDesc_(a, b.getVoip
()) ? i18n.phonenumbers.PhoneNumberType.VOIP : this.isNumberMatchingDesc_(a, b.getPersonalNumber()) ? i18n.phonenumbers.PhoneNumberType
.PERSONAL_NUMBER :
  this.isNumberMatchingDesc_(a, b.getPager()) ? i18n.phonenumbers.PhoneNumberType.PAGER : this.isNumberMatchingDesc_(a, b.getUan
()) ? i18n.phonenumbers.PhoneNumberType.UAN : this.isNumberMatchingDesc_(a, b.getVoicemail()) ? i18n.phonenumbers.PhoneNumberType
.VOICEMAIL : this.isNumberMatchingDesc_(a, b.getFixedLine()) ? b.getSameMobileAndFixedLinePattern() || this.isNumberMatchingDesc_
(a, b.getMobile()) ? i18n.phonenumbers.PhoneNumberType.FIXED_LINE_OR_MOBILE : i18n.phonenumbers.PhoneNumberType.FIXED_LINE :
  !b.getSameMobileAndFixedLinePattern() && this.isNumberMatchingDesc_(a, b.getMobile()) ? i18n.phonenumbers.PhoneNumberType.MOBILE
 : i18n.phonenumbers.PhoneNumberType.UNKNOWN : i18n.phonenumbers.PhoneNumberType.UNKNOWN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getRegionCodeForCountryCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getRegionCodeForCountryCode (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getRegionCodeForCountryCode)
- description and source-code
```javascript
getRegionCodeForCountryCode = function (a) {
  a = i18n.phonenumbers.metadata.countryCodeToRegionCodeMap[a];
  return null == a ? i18n.phonenumbers.PhoneNumberUtil.UNKNOWN_REGION_ : a[0];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getRegionCodeForNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getRegionCodeForNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getRegionCodeForNumber)
- description and source-code
```javascript
getRegionCodeForNumber = function (a) {
  if (null == a) {
    return null;
  }
  var b = a.getCountryCodeOrDefault(), b = i18n.phonenumbers.metadata.countryCodeToRegionCodeMap[b];
  return null == b ? null : 1 == b.length ? b[0] : this.getRegionCodeForNumberFromRegionList_(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getRegionCodeForNumberFromRegionList_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getRegionCodeForNumberFromRegionList_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getRegionCodeForNumberFromRegionList_)
- description and source-code
```javascript
getRegionCodeForNumberFromRegionList_ = function (a, b) {
  for (var c = this.getNationalSignificantNumber(a), d, e = b.length, f = 0;f < e;f++) {
    d = b[f];
    var g = this.getMetadataForRegion(d);
    if (g.hasLeadingDigits()) {
      if (0 == c.search(g.getLeadingDigits())) {
        return d;
      }
    } else {
      if (this.getNumberTypeHelper_(c, g) != i18n.phonenumbers.PhoneNumberType.UNKNOWN) {
        return d;
      }
    }
  }
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getRegionCodesForCountryCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getRegionCodesForCountryCode (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getRegionCodesForCountryCode)
- description and source-code
```javascript
getRegionCodesForCountryCode = function (a) {
  a = i18n.phonenumbers.metadata.countryCodeToRegionCodeMap[a];
  return null == a ? [] : a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getSupportedGlobalNetworkCallingCodes"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getSupportedGlobalNetworkCallingCodes ()](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getSupportedGlobalNetworkCallingCodes)
- description and source-code
```javascript
getSupportedGlobalNetworkCallingCodes = function () {
  var a = goog.array.filter(Object.keys(i18n.phonenumbers.metadata.countryToMetadata), function(a) {
    return !isNaN(a);
  });
  return goog.array.map(a, function(a) {
    return parseInt(a, 10);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getSupportedRegions"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getSupportedRegions ()](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getSupportedRegions)
- description and source-code
```javascript
getSupportedRegions = function () {
  return goog.array.filter(Object.keys(i18n.phonenumbers.metadata.countryToMetadata), function(a) {
    return isNaN(a);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getSupportedTypesForNonGeoEntity"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getSupportedTypesForNonGeoEntity (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getSupportedTypesForNonGeoEntity)
- description and source-code
```javascript
getSupportedTypesForNonGeoEntity = function (a) {
  a = this.getMetadataForNonGeographicalRegion(a);
  return null == a ? [] : i18n.phonenumbers.PhoneNumberUtil.getSupportedTypesForMetadata_(a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getSupportedTypesForRegion"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>getSupportedTypesForRegion (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.getSupportedTypesForRegion)
- description and source-code
```javascript
getSupportedTypesForRegion = function (a) {
  return this.isValidRegionCode_(a) ? i18n.phonenumbers.PhoneNumberUtil.getSupportedTypesForMetadata_(this.getMetadataForRegion(
a)) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.hasFormattingPatternForNumber_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>hasFormattingPatternForNumber_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.hasFormattingPatternForNumber_)
- description and source-code
```javascript
hasFormattingPatternForNumber_ = function (a) {
  var b = a.getCountryCodeOrDefault(), c = this.getRegionCodeForCountryCode(b), b = this.getMetadataForRegionOrCallingCode_(b, c
);
  if (null == b) {
    return !1;
  }
  a = this.getNationalSignificantNumber(a);
  return null != this.chooseFormattingPatternForNumber_(b.numberFormatArray(), a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.hasUnexpectedItalianLeadingZero_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>hasUnexpectedItalianLeadingZero_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.hasUnexpectedItalianLeadingZero_)
- description and source-code
```javascript
hasUnexpectedItalianLeadingZero_ = function (a) {
  return a.hasItalianLeadingZero() && !this.isLeadingZeroPossible(a.getCountryCodeOrDefault());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.hasValidCountryCallingCode_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>hasValidCountryCallingCode_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.hasValidCountryCallingCode_)
- description and source-code
```javascript
hasValidCountryCallingCode_ = function (a) {
  return a in i18n.phonenumbers.metadata.countryCodeToRegionCodeMap;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isAlphaNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isAlphaNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isAlphaNumber)
- description and source-code
```javascript
isAlphaNumber = function (a) {
  if (!i18n.phonenumbers.PhoneNumberUtil.isViablePhoneNumber(a)) {
    return !1;
  }
  a = new goog.string.StringBuffer(a);
  this.maybeStripExtension(a);
  return i18n.phonenumbers.PhoneNumberUtil.matchesEntirely_(i18n.phonenumbers.PhoneNumberUtil.VALID_ALPHA_PHONE_PATTERN_, a.toString
());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isLeadingZeroPossible"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isLeadingZeroPossible (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isLeadingZeroPossible)
- description and source-code
```javascript
isLeadingZeroPossible = function (a) {
  a = this.getMetadataForRegionOrCallingCode_(a, this.getRegionCodeForCountryCode(a));
  return null != a && a.getLeadingZeroPossibleOrDefault();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isNANPACountry"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isNANPACountry (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isNANPACountry)
- description and source-code
```javascript
isNANPACountry = function (a) {
  return null != a && goog.array.contains(i18n.phonenumbers.metadata.countryCodeToRegionCodeMap[i18n.phonenumbers.PhoneNumberUtil
.NANPA_COUNTRY_CODE_], a.toUpperCase());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isNationalNumberSuffixOfTheOther_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isNationalNumberSuffixOfTheOther_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isNationalNumberSuffixOfTheOther_)
- description and source-code
```javascript
isNationalNumberSuffixOfTheOther_ = function (a, b) {
  var c = "" + a.getNationalNumber(), d = "" + b.getNationalNumber();
  return goog.string.endsWith(c, d) || goog.string.endsWith(d, c);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isNumberGeographical"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isNumberGeographical (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isNumberGeographical)
- description and source-code
```javascript
isNumberGeographical = function (a) {
  var b = this.getNumberType(a);
  return b == i18n.phonenumbers.PhoneNumberType.FIXED_LINE || b == i18n.phonenumbers.PhoneNumberType.FIXED_LINE_OR_MOBILE || goog
.array.contains(i18n.phonenumbers.PhoneNumberUtil.GEO_MOBILE_COUNTRIES_, a.getCountryCodeOrDefault()) && b == i18n.phonenumbers.
PhoneNumberType.MOBILE;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isNumberMatch"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isNumberMatch (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isNumberMatch)
- description and source-code
```javascript
isNumberMatch = function (a, b) {
  var c, d;
  if ("string" == typeof a) {
    try {
      c = this.parse(a, i18n.phonenumbers.PhoneNumberUtil.UNKNOWN_REGION_);
    } catch (g) {
      if (g.message != i18n.phonenumbers.Error.INVALID_COUNTRY_CODE) {
        return i18n.phonenumbers.PhoneNumberUtil.MatchType.NOT_A_NUMBER;
      }
      if ("string" != typeof b) {
        var e = this.getRegionCodeForCountryCode(b.getCountryCodeOrDefault());
        if (e != i18n.phonenumbers.PhoneNumberUtil.UNKNOWN_REGION_) {
          try {
            c = this.parse(a, e);
          } catch (h) {
            return i18n.phonenumbers.PhoneNumberUtil.MatchType.NOT_A_NUMBER;
          }
          c = this.isNumberMatch(c, b);
          return c == i18n.phonenumbers.PhoneNumberUtil.MatchType.EXACT_MATCH ? i18n.phonenumbers.PhoneNumberUtil.MatchType.NSN_MATCH
 : c;
        }
      }
      try {
        c = this.parseHelper_(a, null, !1, !1);
      } catch (h) {
        return i18n.phonenumbers.PhoneNumberUtil.MatchType.NOT_A_NUMBER;
      }
    }
  } else {
    c = a.clone();
  }
  if ("string" == typeof b) {
    try {
      return d = this.parse(b, i18n.phonenumbers.PhoneNumberUtil.UNKNOWN_REGION_), this.isNumberMatch(a, d);
    } catch (g) {
      return g.message != i18n.phonenumbers.Error.INVALID_COUNTRY_CODE ? i18n.phonenumbers.PhoneNumberUtil.MatchType.NOT_A_NUMBER
 : this.isNumberMatch(b, c);
    }
  } else {
    d = b.clone();
  }
  c = i18n.phonenumbers.PhoneNumberUtil.copyCoreFieldsOnly_(c);
  d = i18n.phonenumbers.PhoneNumberUtil.copyCoreFieldsOnly_(d);
  if (c.hasExtension() && d.hasExtension() && c.getExtension() != d.getExtension()) {
    return i18n.phonenumbers.PhoneNumberUtil.MatchType.NO_MATCH;
  }
  var e = c.getCountryCodeOrDefault(), f = d.getCountryCodeOrDefault();
  if (0 != e && 0 != f) {
    return c.equals(d) ? i18n.phonenumbers.PhoneNumberUtil.MatchType.EXACT_MATCH : e == f && this.isNationalNumberSuffixOfTheOther_
(c, d) ? i18n.phonenumbers.PhoneNumberUtil.MatchType.SHORT_NSN_MATCH : i18n.phonenumbers.PhoneNumberUtil.MatchType.NO_MATCH;
  }
  c.setCountryCode(0);
  d.setCountryCode(0);
  return c.equals(d) ? i18n.phonenumbers.PhoneNumberUtil.MatchType.NSN_MATCH : this.isNationalNumberSuffixOfTheOther_(c, d) ? i18n
.phonenumbers.PhoneNumberUtil.MatchType.SHORT_NSN_MATCH : i18n.phonenumbers.PhoneNumberUtil.MatchType.NO_MATCH;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isNumberMatchingDesc_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isNumberMatchingDesc_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isNumberMatchingDesc_)
- description and source-code
```javascript
isNumberMatchingDesc_ = function (a, b) {
  var c = a.length;
  return 0 < b.possibleLengthCount() && -1 == goog.array.indexOf(b.possibleLengthArray(), c) ? !1 : i18n.phonenumbers.PhoneNumberUtil
.matchesEntirely_(b.getNationalNumberPatternOrDefault(), a);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isPossibleNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isPossibleNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isPossibleNumber)
- description and source-code
```javascript
isPossibleNumber = function (a) {
  return this.isPossibleNumberWithReason(a) == i18n.phonenumbers.PhoneNumberUtil.ValidationResult.IS_POSSIBLE;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isPossibleNumberForType"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isPossibleNumberForType (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isPossibleNumberForType)
- description and source-code
```javascript
isPossibleNumberForType = function (a, b) {
  return this.isPossibleNumberForTypeWithReason(a, b) == i18n.phonenumbers.PhoneNumberUtil.ValidationResult.IS_POSSIBLE;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isPossibleNumberForTypeWithReason"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isPossibleNumberForTypeWithReason (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isPossibleNumberForTypeWithReason)
- description and source-code
```javascript
isPossibleNumberForTypeWithReason = function (a, b) {
  var c = this.getNationalSignificantNumber(a), d = a.getCountryCodeOrDefault();
  if (!this.hasValidCountryCallingCode_(d)) {
    return i18n.phonenumbers.PhoneNumberUtil.ValidationResult.INVALID_COUNTRY_CODE;
  }
  var e = this.getRegionCodeForCountryCode(d), d = this.getMetadataForRegionOrCallingCode_(d, e);
  return this.testNumberLengthForType_(c, d, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isPossibleNumberString"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isPossibleNumberString (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isPossibleNumberString)
- description and source-code
```javascript
isPossibleNumberString = function (a, b) {
  try {
    return this.isPossibleNumber(this.parse(a, b));
  } catch (c) {
    return !1;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isPossibleNumberWithReason"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isPossibleNumberWithReason (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isPossibleNumberWithReason)
- description and source-code
```javascript
isPossibleNumberWithReason = function (a) {
  return this.isPossibleNumberForTypeWithReason(a, i18n.phonenumbers.PhoneNumberType.UNKNOWN);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isValidNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isValidNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isValidNumber)
- description and source-code
```javascript
isValidNumber = function (a) {
  var b = this.getRegionCodeForNumber(a);
  return this.isValidNumberForRegion(a, b);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isValidNumberForRegion"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isValidNumberForRegion (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isValidNumberForRegion)
- description and source-code
```javascript
isValidNumberForRegion = function (a, b) {
  var c = a.getCountryCodeOrDefault(), d = this.getMetadataForRegionOrCallingCode_(c, b);
  if (null == d || i18n.phonenumbers.PhoneNumberUtil.REGION_CODE_FOR_NON_GEO_ENTITY != b && c != this.getCountryCodeForValidRegion_
(b)) {
    return !1;
  }
  c = this.getNationalSignificantNumber(a);
  return this.getNumberTypeHelper_(c, d) != i18n.phonenumbers.PhoneNumberType.UNKNOWN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isValidRegionCode_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>isValidRegionCode_ (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.isValidRegionCode_)
- description and source-code
```javascript
isValidRegionCode_ = function (a) {
  return null != a && isNaN(a) && a.toUpperCase() in i18n.phonenumbers.metadata.countryToMetadata;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.maybeExtractCountryCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>maybeExtractCountryCode (a, b, c, d, e)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.maybeExtractCountryCode)
- description and source-code
```javascript
maybeExtractCountryCode = function (a, b, c, d, e) {
  if (0 == a.length) {
    return 0;
  }
  a = new goog.string.StringBuffer(a);
  var f;
  null != b && (f = b.getInternationalPrefix());
  null == f && (f = "NonMatch");
  f = this.maybeStripInternationalPrefixAndNormalize(a, f);
  d && e.setCountryCodeSource(f);
  if (f != i18n.phonenumbers.PhoneNumber.CountryCodeSource.FROM_DEFAULT_COUNTRY) {
    if (a.getLength() <= i18n.phonenumbers.PhoneNumberUtil.MIN_LENGTH_FOR_NSN_) {
      throw Error(i18n.phonenumbers.Error.TOO_SHORT_AFTER_IDD);
    }
    b = this.extractCountryCode(a, c);
    if (0 != b) {
      return e.setCountryCode(b), b;
    }
    throw Error(i18n.phonenumbers.Error.INVALID_COUNTRY_CODE);
  }
  if (null != b) {
    f = b.getCountryCodeOrDefault();
    var g = "" + f, h = a.toString();
    if (goog.string.startsWith(h, g) && (g = new goog.string.StringBuffer(h.substring(g.length)), h = b.getGeneralDesc(), h = new
 RegExp(h.getNationalNumberPatternOrDefault()), this.maybeStripNationalPrefixAndCarrierCode(g, b, null), g = g.toString(), !i18n
.phonenumbers.PhoneNumberUtil.matchesEntirely_(h, a.toString()) && i18n.phonenumbers.PhoneNumberUtil.matchesEntirely_(h, g) || this
.testNumberLength_(a.toString(), b) == i18n.phonenumbers.PhoneNumberUtil.ValidationResult.TOO_LONG)) {
      return c.append(g), d && e.setCountryCodeSource(i18n.phonenumbers.PhoneNumber.CountryCodeSource.FROM_NUMBER_WITHOUT_PLUS_SIGN
), e.setCountryCode(f), f;
    }
  }
  e.setCountryCode(0);
  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.maybeGetFormattedExtension_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>maybeGetFormattedExtension_ (a, b, c)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.maybeGetFormattedExtension_)
- description and source-code
```javascript
maybeGetFormattedExtension_ = function (a, b, c) {
  return a.hasExtension() && 0 != a.getExtension().length ? c == i18n.phonenumbers.PhoneNumberFormat.RFC3966 ? i18n.phonenumbers
.PhoneNumberUtil.RFC3966_EXTN_PREFIX_ + a.getExtension() : b.hasPreferredExtnPrefix() ? b.getPreferredExtnPrefix() + a.getExtensionOrDefault
() : i18n.phonenumbers.PhoneNumberUtil.DEFAULT_EXTN_PREFIX_ + a.getExtensionOrDefault() : "";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.maybeStripExtension"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>maybeStripExtension (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.maybeStripExtension)
- description and source-code
```javascript
maybeStripExtension = function (a) {
  var b = a.toString(), c = b.search(i18n.phonenumbers.PhoneNumberUtil.EXTN_PATTERN_);
  if (0 <= c && i18n.phonenumbers.PhoneNumberUtil.isViablePhoneNumber(b.substring(0, c))) {
    for (var d = b.match(i18n.phonenumbers.PhoneNumberUtil.EXTN_PATTERN_), e = d.length, f = 1;f < e;++f) {
      if (null != d[f] && 0 < d[f].length) {
        return a.clear(), a.append(b.substring(0, c)), d[f];
      }
    }
  }
  return "";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.maybeStripInternationalPrefixAndNormalize"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>maybeStripInternationalPrefixAndNormalize (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.maybeStripInternationalPrefixAndNormalize)
- description and source-code
```javascript
maybeStripInternationalPrefixAndNormalize = function (a, b) {
  var c = a.toString();
  if (0 == c.length) {
    return i18n.phonenumbers.PhoneNumber.CountryCodeSource.FROM_DEFAULT_COUNTRY;
  }
  if (i18n.phonenumbers.PhoneNumberUtil.LEADING_PLUS_CHARS_PATTERN_.test(c)) {
    return c = c.replace(i18n.phonenumbers.PhoneNumberUtil.LEADING_PLUS_CHARS_PATTERN_, ""), a.clear(), a.append(i18n.phonenumbers
.PhoneNumberUtil.normalize(c)), i18n.phonenumbers.PhoneNumber.CountryCodeSource.FROM_NUMBER_WITH_PLUS_SIGN;
  }
  c = new RegExp(b);
  i18n.phonenumbers.PhoneNumberUtil.normalizeSB_(a);
  return this.parsePrefixAsIdd_(c, a) ? i18n.phonenumbers.PhoneNumber.CountryCodeSource.FROM_NUMBER_WITH_IDD : i18n.phonenumbers
.PhoneNumber.CountryCodeSource.FROM_DEFAULT_COUNTRY;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.maybeStripNationalPrefixAndCarrierCode"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>maybeStripNationalPrefixAndCarrierCode (a, b, c)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.maybeStripNationalPrefixAndCarrierCode)
- description and source-code
```javascript
maybeStripNationalPrefixAndCarrierCode = function (a, b, c) {
  var d = a.toString(), e = d.length, f = b.getNationalPrefixForParsing();
  if (0 == e || null == f || 0 == f.length) {
    return !1;
  }
  var g = new RegExp("^(?:" + f + ")");
  if (e = g.exec(d)) {
    var f = new RegExp(b.getGeneralDesc().getNationalNumberPatternOrDefault()), h = i18n.phonenumbers.PhoneNumberUtil.matchesEntirely_
(f, d), k = e.length - 1;
    b = b.getNationalPrefixTransformRule();
    if (null == b || 0 == b.length || null == e[k] || 0 == e[k].length) {
      if (h && !i18n.phonenumbers.PhoneNumberUtil.matchesEntirely_(f, d.substring(e[0].length))) {
        return !1;
      }
      null != c && 0 < k && null != e[k] && c.append(e[1]);
      a.set(d.substring(e[0].length));
    } else {
      d = d.replace(g, b);
      if (h && !i18n.phonenumbers.PhoneNumberUtil.matchesEntirely_(f, d)) {
        return !1;
      }
      null != c && 0 < k && c.append(e[1]);
      a.set(d);
    }
    return !0;
  }
  return !1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.parse"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>parse (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.parse)
- description and source-code
```javascript
parse = function (a, b) {
  return this.parseHelper_(a, b, !1, !0);
}
```
- example usage
```shell
...
// Require 'PhoneNumberFormat'.
var PNF = require('google-libphonenumber').PhoneNumberFormat;

// Get an instance of 'PhoneNumberUtil'.
var phoneUtil = require('google-libphonenumber').PhoneNumberUtil.getInstance();

// Parse number with country code.
var phoneNumber = phoneUtil.parse('202-456-1414', 'US');

// Print number in the international format.
console.log(phoneUtil.format(phoneNumber, PNF.INTERNATIONAL));
// => +1 202-456-1414
'''

#### Using the "As You Type" Formatter
...
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.parseAndKeepRawInput"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>parseAndKeepRawInput (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.parseAndKeepRawInput)
- description and source-code
```javascript
parseAndKeepRawInput = function (a, b) {
  if (!this.isValidRegionCode_(b) && 0 < a.length && a.charAt(0) != i18n.phonenumbers.PhoneNumberUtil.PLUS_SIGN) {
    throw Error(i18n.phonenumbers.Error.INVALID_COUNTRY_CODE);
  }
  return this.parseHelper_(a, b, !0, !0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.parseHelper_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>parseHelper_ (a, b, c, d)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.parseHelper_)
- description and source-code
```javascript
parseHelper_ = function (a, b, c, d) {
  if (null == a) {
    throw Error(i18n.phonenumbers.Error.NOT_A_NUMBER);
  }
  if (a.length > i18n.phonenumbers.PhoneNumberUtil.MAX_INPUT_STRING_LENGTH_) {
    throw Error(i18n.phonenumbers.Error.TOO_LONG);
  }
  var e = new goog.string.StringBuffer;
  this.buildNationalNumberForParsing_(a, e);
  if (!i18n.phonenumbers.PhoneNumberUtil.isViablePhoneNumber(e.toString())) {
    throw Error(i18n.phonenumbers.Error.NOT_A_NUMBER);
  }
  if (d && !this.checkRegionForParsing_(e.toString(), b)) {
    throw Error(i18n.phonenumbers.Error.INVALID_COUNTRY_CODE);
  }
  d = new i18n.phonenumbers.PhoneNumber;
  c && d.setRawInput(a);
  a = this.maybeStripExtension(e);
  0 < a.length && d.setExtension(a);
  a = this.getMetadataForRegion(b);
  var f = new goog.string.StringBuffer, g = 0, h = e.toString();
  try {
    g = this.maybeExtractCountryCode(h, a, f, c, d);
  } catch (k) {
    if (k.message == i18n.phonenumbers.Error.INVALID_COUNTRY_CODE && i18n.phonenumbers.PhoneNumberUtil.LEADING_PLUS_CHARS_PATTERN_
.test(h)) {
      if (h = h.replace(i18n.phonenumbers.PhoneNumberUtil.LEADING_PLUS_CHARS_PATTERN_, ""), g = this.maybeExtractCountryCode(h,
a, f, c, d), 0 == g) {
        throw k;
      }
    } else {
      throw k;
    }
  }
  0 != g ? (e = this.getRegionCodeForCountryCode(g), e != b && (a = this.getMetadataForRegionOrCallingCode_(g, e))) : (i18n.phonenumbers
.PhoneNumberUtil.normalizeSB_(e), f.append(e.toString()), null != b ? (g = a.getCountryCodeOrDefault(), d.setCountryCode(g)) : c
 && d.clearCountryCodeSource());
  if (f.getLength() < i18n.phonenumbers.PhoneNumberUtil.MIN_LENGTH_FOR_NSN_) {
    throw Error(i18n.phonenumbers.Error.TOO_SHORT_NSN);
  }
  null != a && (b = new goog.string.StringBuffer, e = new goog.string.StringBuffer(f.toString()), this.maybeStripNationalPrefixAndCarrierCode
(e, a, b), this.testNumberLength_(e.toString(), a) != i18n.phonenumbers.PhoneNumberUtil.ValidationResult.TOO_SHORT && (f = e, c &&
0 < b.toString().length && d.setPreferredDomesticCarrierCode(b.toString())));
  c = f.toString();
  b = c.length;
  if (b < i18n.phonenumbers.PhoneNumberUtil.MIN_LENGTH_FOR_NSN_) {
    throw Error(i18n.phonenumbers.Error.TOO_SHORT_NSN);
  }
  if (b > i18n.phonenumbers.PhoneNumberUtil.MAX_LENGTH_FOR_NSN_) {
    throw Error(i18n.phonenumbers.Error.TOO_LONG);
  }
  i18n.phonenumbers.PhoneNumberUtil.setItalianLeadingZerosForPhoneNumber_(c, d);
  d.setNationalNumber(parseInt(c, 10));
  return d;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.parsePrefixAsIdd_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>parsePrefixAsIdd_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.parsePrefixAsIdd_)
- description and source-code
```javascript
parsePrefixAsIdd_ = function (a, b) {
  var c = b.toString();
  if (0 == c.search(a)) {
    var d = c.match(a)[0].length, e = c.substring(d).match(i18n.phonenumbers.PhoneNumberUtil.CAPTURING_DIGIT_PATTERN);
    if (e && null != e[1] && 0 < e[1].length && "0" == i18n.phonenumbers.PhoneNumberUtil.normalizeDigitsOnly(e[1])) {
      return !1;
    }
    b.clear();
    b.append(c.substring(d));
    return !0;
  }
  return !1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.prefixNumberWithCountryCallingCode_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>prefixNumberWithCountryCallingCode_ (a, b, c, d)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.prefixNumberWithCountryCallingCode_)
- description and source-code
```javascript
prefixNumberWithCountryCallingCode_ = function (a, b, c, d) {
  switch(b) {
    case i18n.phonenumbers.PhoneNumberFormat.E164:
      return i18n.phonenumbers.PhoneNumberUtil.PLUS_SIGN + a + c + d;
    case i18n.phonenumbers.PhoneNumberFormat.INTERNATIONAL:
      return i18n.phonenumbers.PhoneNumberUtil.PLUS_SIGN + a + " " + c + d;
    case i18n.phonenumbers.PhoneNumberFormat.RFC3966:
      return i18n.phonenumbers.PhoneNumberUtil.RFC3966_PREFIX_ + i18n.phonenumbers.PhoneNumberUtil.PLUS_SIGN + a + "-" + c + d;
    default:
      return c + d;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.rawInputContainsNationalPrefix_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>rawInputContainsNationalPrefix_ (a, b, c)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.rawInputContainsNationalPrefix_)
- description and source-code
```javascript
rawInputContainsNationalPrefix_ = function (a, b, c) {
  a = i18n.phonenumbers.PhoneNumberUtil.normalizeDigitsOnly(a);
  if (goog.string.startsWith(a, b)) {
    try {
      return this.isValidNumber(this.parse(a.substring(b.length), c));
    } catch (d) {
    }
  }
  return !1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.testNumberLengthForType_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>testNumberLengthForType_ (a, b, c)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.testNumberLengthForType_)
- description and source-code
```javascript
testNumberLengthForType_ = function (a, b, c) {
  var d = i18n.phonenumbers.PhoneNumberUtil.getNumberDescByType_(b, c), e = 0 == d.possibleLengthCount() ? b.getGeneralDesc().possibleLengthArray
() : d.possibleLengthArray(), d = d.possibleLengthLocalOnlyArray();
  if (c == i18n.phonenumbers.PhoneNumberType.FIXED_LINE_OR_MOBILE) {
    if (i18n.phonenumbers.PhoneNumberUtil.descHasPossibleNumberData_(i18n.phonenumbers.PhoneNumberUtil.getNumberDescByType_(b, i18n
.phonenumbers.PhoneNumberType.FIXED_LINE))) {
      c = i18n.phonenumbers.PhoneNumberUtil.getNumberDescByType_(b, i18n.phonenumbers.PhoneNumberType.MOBILE), i18n.phonenumbers
.PhoneNumberUtil.descHasPossibleNumberData_(c) && (e = e.concat(0 == c.possibleLengthCount() ? b.getGeneralDesc().possibleLengthArray
() : c.possibleLengthArray()), goog.array.sort(e), 0 == d.length ? d = c.possibleLengthLocalOnlyArray() : (d = d.concat(c.possibleLengthLocalOnlyArray
()), goog.array.sort(d)));
    } else {
      return this.testNumberLengthForType_(a, b, i18n.phonenumbers.PhoneNumberType.MOBILE);
    }
  }
  if (-1 == e[0]) {
    return i18n.phonenumbers.PhoneNumberUtil.ValidationResult.INVALID_LENGTH;
  }
  a = a.length;
  if (-1 < goog.array.indexOf(d, a)) {
    return i18n.phonenumbers.PhoneNumberUtil.ValidationResult.IS_POSSIBLE;
  }
  b = e[0];
  return b == a ? i18n.phonenumbers.PhoneNumberUtil.ValidationResult.IS_POSSIBLE : b > a ? i18n.phonenumbers.PhoneNumberUtil.ValidationResult
.TOO_SHORT : e[e.length - 1] < a ? i18n.phonenumbers.PhoneNumberUtil.ValidationResult.TOO_LONG : -1 < goog.array.indexOf(e, a, 1
) ? i18n.phonenumbers.PhoneNumberUtil.ValidationResult.IS_POSSIBLE : i18n.phonenumbers.PhoneNumberUtil.ValidationResult.TOO_LONG
;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.testNumberLength_"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>testNumberLength_ (a, b)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.testNumberLength_)
- description and source-code
```javascript
testNumberLength_ = function (a, b) {
  return this.testNumberLengthForType_(a, b, i18n.phonenumbers.PhoneNumberType.UNKNOWN);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.truncateTooLongNumber"></a>[function <span class="apidocSignatureSpan">google-libphonenumber.PhoneNumberUtil.prototype.</span>truncateTooLongNumber (a)](#apidoc.element.google-libphonenumber.PhoneNumberUtil.prototype.truncateTooLongNumber)
- description and source-code
```javascript
truncateTooLongNumber = function (a) {
  if (this.isValidNumber(a)) {
    return !0;
  }
  var b = a.clone(), c = a.getNationalNumberOrDefault();
  do {
    if (c = Math.floor(c / 10), b.setNationalNumber(c), 0 == c || this.isPossibleNumberWithReason(b) == i18n.phonenumbers.PhoneNumberUtil
.ValidationResult.TOO_SHORT) {
      return !1;
    }
  } while (!this.isValidNumber(b));
  a.setNationalNumber(c);
  return !0;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
