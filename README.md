# api documentation for  [inquirer (v3.0.6)](https://github.com/sboudrias/Inquirer.js#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-inquirer.svg)](https://travis-ci.org/npmdoc/node-npmdoc-inquirer)
#### A collection of common interactive command line user interfaces.

[![NPM](https://nodei.co/npm/inquirer.png?downloads=true)](https://www.npmjs.com/package/inquirer)

[![apidoc](https://npmdoc.github.io/node-npmdoc-inquirer/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-inquirer_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-inquirer/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-inquirer/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Simon Boudrias",
        "email": "admin@simonboudrias.com"
    },
    "bugs": {
        "url": "https://github.com/sboudrias/Inquirer.js/issues"
    },
    "dependencies": {
        "ansi-escapes": "^1.1.0",
        "chalk": "^1.0.0",
        "cli-cursor": "^2.1.0",
        "cli-width": "^2.0.0",
        "external-editor": "^2.0.1",
        "figures": "^2.0.0",
        "lodash": "^4.3.0",
        "mute-stream": "0.0.7",
        "run-async": "^2.2.0",
        "rx": "^4.1.0",
        "string-width": "^2.0.0",
        "strip-ansi": "^3.0.0",
        "through": "^2.3.6"
    },
    "description": "A collection of common interactive command line user interfaces.",
    "devDependencies": {
        "chai": "^3.0.0",
        "cmdify": "^0.0.4",
        "eslint": "^3.10.2",
        "eslint-config-xo-space": "^0.15.0",
        "gulp": "^3.9.0",
        "gulp-coveralls": "^0.1.0",
        "gulp-eslint": "^3.0.1",
        "gulp-exclude-gitignore": "^1.0.0",
        "gulp-istanbul": "^1.1.1",
        "gulp-line-ending-corrector": "^1.0.1",
        "gulp-mocha": "^3.0.0",
        "gulp-nsp": "^2.1.0",
        "gulp-plumber": "^1.0.0",
        "mocha": "^3.1.2",
        "mockery": "^2.0.0",
        "sinon": "^1.12.1"
    },
    "directories": {},
    "dist": {
        "shasum": "e04aaa9d05b7a3cb9b0f407d04375f0447190347",
        "tarball": "https://registry.npmjs.org/inquirer/-/inquirer-3.0.6.tgz"
    },
    "eslintConfig": {
        "extends": "xo-space",
        "env": {
            "mocha": true
        },
        "rules": {
            "quotes": [
                "error",
                "single"
            ],
            "no-unused-expressions": "off",
            "handle-callback-err": "off",
            "no-eq-null": "off",
            "eqeqeq": [
                "error",
                "allow-null"
            ]
        }
    },
    "files": [
        "lib"
    ],
    "gitHead": "6fa46107c940bc8fb7ff66191538ed54e181e166",
    "homepage": "https://github.com/sboudrias/Inquirer.js#readme",
    "keywords": [
        "command",
        "prompt",
        "stdin",
        "cli",
        "tty",
        "menu"
    ],
    "license": "MIT",
    "main": "lib/inquirer.js",
    "maintainers": [
        {
            "name": "mischah",
            "email": "mail@michael-kuehnel.de"
        },
        {
            "name": "sboudrias",
            "email": "admin@simonboudrias.com"
        }
    ],
    "name": "inquirer",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/sboudrias/Inquirer.js.git"
    },
    "scripts": {
        "prepublish": "gulp prepublish",
        "test": "gulp"
    },
    "version": "3.0.6"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module inquirer](#apidoc.module.inquirer)
1.  [function <span class="apidocSignatureSpan">inquirer.</span>Separator (line)](#apidoc.element.inquirer.Separator)
1.  [function <span class="apidocSignatureSpan">inquirer.</span>createPromptModule (opt)](#apidoc.element.inquirer.createPromptModule)
1.  [function <span class="apidocSignatureSpan">inquirer.</span>prompt (questions)](#apidoc.element.inquirer.prompt)
1.  [function <span class="apidocSignatureSpan">inquirer.</span>registerPrompt (name, prompt)](#apidoc.element.inquirer.registerPrompt)
1.  [function <span class="apidocSignatureSpan">inquirer.</span>restoreDefaultPrompts ()](#apidoc.element.inquirer.restoreDefaultPrompts)
1.  [function <span class="apidocSignatureSpan">inquirer.</span>ui.BottomBar (opt)](#apidoc.element.inquirer.ui.BottomBar)
1.  [function <span class="apidocSignatureSpan">inquirer.</span>ui.Prompt (prompts, opt)](#apidoc.element.inquirer.ui.Prompt)
1.  object <span class="apidocSignatureSpan">inquirer.</span>Separator.prototype
1.  object <span class="apidocSignatureSpan">inquirer.</span>prompt.prompts
1.  object <span class="apidocSignatureSpan">inquirer.</span>prompt.prompts.checkbox.prototype
1.  object <span class="apidocSignatureSpan">inquirer.</span>prompt.prompts.confirm.prototype
1.  object <span class="apidocSignatureSpan">inquirer.</span>prompt.prompts.editor.prototype
1.  object <span class="apidocSignatureSpan">inquirer.</span>prompt.prompts.expand.prototype
1.  object <span class="apidocSignatureSpan">inquirer.</span>prompt.prompts.input.prototype
1.  object <span class="apidocSignatureSpan">inquirer.</span>prompt.prompts.list.prototype
1.  object <span class="apidocSignatureSpan">inquirer.</span>prompt.prompts.password.prototype
1.  object <span class="apidocSignatureSpan">inquirer.</span>prompt.prompts.rawlist.prototype
1.  object <span class="apidocSignatureSpan">inquirer.</span>prompts
1.  object <span class="apidocSignatureSpan">inquirer.</span>ui
1.  object <span class="apidocSignatureSpan">inquirer.</span>ui.BottomBar.prototype
1.  object <span class="apidocSignatureSpan">inquirer.</span>ui.BottomBar.super_.prototype
1.  object <span class="apidocSignatureSpan">inquirer.</span>ui.Prompt.prototype

#### [module inquirer.Separator](#apidoc.module.inquirer.Separator)
1.  [function <span class="apidocSignatureSpan">inquirer.</span>Separator (line)](#apidoc.element.inquirer.Separator.Separator)
1.  [function <span class="apidocSignatureSpan">inquirer.Separator.</span>exclude (obj)](#apidoc.element.inquirer.Separator.exclude)

#### [module inquirer.Separator.prototype](#apidoc.module.inquirer.Separator.prototype)
1.  [function <span class="apidocSignatureSpan">inquirer.Separator.prototype.</span>toString ()](#apidoc.element.inquirer.Separator.prototype.toString)

#### [module inquirer.prompt](#apidoc.module.inquirer.prompt)
1.  [function <span class="apidocSignatureSpan">inquirer.</span>prompt (questions)](#apidoc.element.inquirer.prompt.prompt)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.</span>registerPrompt (name, prompt)](#apidoc.element.inquirer.prompt.registerPrompt)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.</span>restoreDefaultPrompts ()](#apidoc.element.inquirer.prompt.restoreDefaultPrompts)
1.  object <span class="apidocSignatureSpan">inquirer.prompt.</span>prompts

#### [module inquirer.prompt.prompts](#apidoc.module.inquirer.prompt.prompts)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.</span>checkbox ()](#apidoc.element.inquirer.prompt.prompts.checkbox)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.</span>confirm ()](#apidoc.element.inquirer.prompt.prompts.confirm)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.</span>editor ()](#apidoc.element.inquirer.prompt.prompts.editor)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.</span>expand ()](#apidoc.element.inquirer.prompt.prompts.expand)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.</span>input ()](#apidoc.element.inquirer.prompt.prompts.input)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.</span>list ()](#apidoc.element.inquirer.prompt.prompts.list)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.</span>password ()](#apidoc.element.inquirer.prompt.prompts.password)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.</span>rawlist ()](#apidoc.element.inquirer.prompt.prompts.rawlist)

#### [module inquirer.prompt.prompts.checkbox.prototype](#apidoc.module.inquirer.prompt.prompts.checkbox.prototype)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>_run (cb)](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype._run)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>getCurrentValue ()](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.getCurrentValue)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>onAllKey ()](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onAllKey)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>onDownKey ()](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onDownKey)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>onEnd (state)](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onEnd)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>onError (state)](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onError)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>onInverseKey ()](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onInverseKey)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>onNumberKey (input)](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onNumberKey)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>onSpaceKey ()](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onSpaceKey)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>onUpKey ()](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onUpKey)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>render (error)](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.render)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>toggleChoice (index)](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.toggleChoice)

#### [module inquirer.prompt.prompts.confirm.prototype](#apidoc.module.inquirer.prompt.prompts.confirm.prototype)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.confirm.prototype.</span>_run (cb)](#apidoc.element.inquirer.prompt.prompts.confirm.prototype._run)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.confirm.prototype.</span>onEnd (input)](#apidoc.element.inquirer.prompt.prompts.confirm.prototype.onEnd)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.confirm.prototype.</span>onKeypress ()](#apidoc.element.inquirer.prompt.prompts.confirm.prototype.onKeypress)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.confirm.prototype.</span>render (answer)](#apidoc.element.inquirer.prompt.prompts.confirm.prototype.render)

#### [module inquirer.prompt.prompts.editor.prototype](#apidoc.module.inquirer.prompt.prompts.editor.prototype)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.editor.prototype.</span>_run (cb)](#apidoc.element.inquirer.prompt.prompts.editor.prototype._run)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.editor.prototype.</span>endExternalEditor (error, result)](#apidoc.element.inquirer.prompt.prompts.editor.prototype.endExternalEditor)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.editor.prototype.</span>onEnd (state)](#apidoc.element.inquirer.prompt.prompts.editor.prototype.onEnd)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.editor.prototype.</span>onError (state)](#apidoc.element.inquirer.prompt.prompts.editor.prototype.onError)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.editor.prototype.</span>render (error)](#apidoc.element.inquirer.prompt.prompts.editor.prototype.render)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.editor.prototype.</span>startExternalEditor ()](#apidoc.element.inquirer.prompt.prompts.editor.prototype.startExternalEditor)

#### [module inquirer.prompt.prompts.expand.prototype](#apidoc.module.inquirer.prompt.prompts.expand.prototype)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.expand.prototype.</span>_run (cb)](#apidoc.element.inquirer.prompt.prompts.expand.prototype._run)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.expand.prototype.</span>generateChoicesString (choices, defaultIndex)](#apidoc.element.inquirer.prompt.prompts.expand.prototype.generateChoicesString)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.expand.prototype.</span>getChoices ()](#apidoc.element.inquirer.prompt.prompts.expand.prototype.getChoices)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.expand.prototype.</span>getCurrentValue (input)](#apidoc.element.inquirer.prompt.prompts.expand.prototype.getCurrentValue)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.expand.prototype.</span>onError (state)](#apidoc.element.inquirer.prompt.prompts.expand.prototype.onError)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.expand.prototype.</span>onKeypress ()](#apidoc.element.inquirer.prompt.prompts.expand.prototype.onKeypress)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.expand.prototype.</span>onSubmit (state)](#apidoc.element.inquirer.prompt.prompts.expand.prototype.onSubmit)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.expand.prototype.</span>render (error, hint)](#apidoc.element.inquirer.prompt.prompts.expand.prototype.render)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.expand.prototype.</span>validateChoices (choices)](#apidoc.element.inquirer.prompt.prompts.expand.prototype.validateChoices)

#### [module inquirer.prompt.prompts.input.prototype](#apidoc.module.inquirer.prompt.prompts.input.prototype)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.input.prototype.</span>_run (cb)](#apidoc.element.inquirer.prompt.prompts.input.prototype._run)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.input.prototype.</span>filterInput (input)](#apidoc.element.inquirer.prompt.prompts.input.prototype.filterInput)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.input.prototype.</span>onEnd (state)](#apidoc.element.inquirer.prompt.prompts.input.prototype.onEnd)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.input.prototype.</span>onError (state)](#apidoc.element.inquirer.prompt.prompts.input.prototype.onError)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.input.prototype.</span>onKeypress ()](#apidoc.element.inquirer.prompt.prompts.input.prototype.onKeypress)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.input.prototype.</span>render (error)](#apidoc.element.inquirer.prompt.prompts.input.prototype.render)

#### [module inquirer.prompt.prompts.list.prototype](#apidoc.module.inquirer.prompt.prompts.list.prototype)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.list.prototype.</span>_run (cb)](#apidoc.element.inquirer.prompt.prompts.list.prototype._run)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.list.prototype.</span>getCurrentValue ()](#apidoc.element.inquirer.prompt.prompts.list.prototype.getCurrentValue)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.list.prototype.</span>onDownKey ()](#apidoc.element.inquirer.prompt.prompts.list.prototype.onDownKey)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.list.prototype.</span>onNumberKey (input)](#apidoc.element.inquirer.prompt.prompts.list.prototype.onNumberKey)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.list.prototype.</span>onSubmit (value)](#apidoc.element.inquirer.prompt.prompts.list.prototype.onSubmit)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.list.prototype.</span>onUpKey ()](#apidoc.element.inquirer.prompt.prompts.list.prototype.onUpKey)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.list.prototype.</span>render ()](#apidoc.element.inquirer.prompt.prompts.list.prototype.render)

#### [module inquirer.prompt.prompts.password.prototype](#apidoc.module.inquirer.prompt.prompts.password.prototype)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.password.prototype.</span>_run (cb)](#apidoc.element.inquirer.prompt.prompts.password.prototype._run)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.password.prototype.</span>filterInput (input)](#apidoc.element.inquirer.prompt.prompts.password.prototype.filterInput)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.password.prototype.</span>onEnd (state)](#apidoc.element.inquirer.prompt.prompts.password.prototype.onEnd)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.password.prototype.</span>onError (state)](#apidoc.element.inquirer.prompt.prompts.password.prototype.onError)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.password.prototype.</span>onKeypress ()](#apidoc.element.inquirer.prompt.prompts.password.prototype.onKeypress)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.password.prototype.</span>render (error)](#apidoc.element.inquirer.prompt.prompts.password.prototype.render)

#### [module inquirer.prompt.prompts.rawlist.prototype](#apidoc.module.inquirer.prompt.prompts.rawlist.prototype)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.rawlist.prototype.</span>_run (cb)](#apidoc.element.inquirer.prompt.prompts.rawlist.prototype._run)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.rawlist.prototype.</span>getCurrentValue (index)](#apidoc.element.inquirer.prompt.prompts.rawlist.prototype.getCurrentValue)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.rawlist.prototype.</span>onEnd (state)](#apidoc.element.inquirer.prompt.prompts.rawlist.prototype.onEnd)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.rawlist.prototype.</span>onError ()](#apidoc.element.inquirer.prompt.prompts.rawlist.prototype.onError)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.rawlist.prototype.</span>onKeypress ()](#apidoc.element.inquirer.prompt.prompts.rawlist.prototype.onKeypress)
1.  [function <span class="apidocSignatureSpan">inquirer.prompt.prompts.rawlist.prototype.</span>render (error)](#apidoc.element.inquirer.prompt.prompts.rawlist.prototype.render)

#### [module inquirer.ui](#apidoc.module.inquirer.ui)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.</span>BottomBar (opt)](#apidoc.element.inquirer.ui.BottomBar)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.</span>Prompt (prompts, opt)](#apidoc.element.inquirer.ui.Prompt)

#### [module inquirer.ui.BottomBar](#apidoc.module.inquirer.ui.BottomBar)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.</span>BottomBar (opt)](#apidoc.element.inquirer.ui.BottomBar.BottomBar)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.BottomBar.</span>super_ (opt)](#apidoc.element.inquirer.ui.BottomBar.super_)

#### [module inquirer.ui.BottomBar.prototype](#apidoc.module.inquirer.ui.BottomBar.prototype)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.BottomBar.prototype.</span>clean ()](#apidoc.element.inquirer.ui.BottomBar.prototype.clean)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.BottomBar.prototype.</span>enforceLF (str)](#apidoc.element.inquirer.ui.BottomBar.prototype.enforceLF)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.BottomBar.prototype.</span>render ()](#apidoc.element.inquirer.ui.BottomBar.prototype.render)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.BottomBar.prototype.</span>updateBottomBar (bottomBar)](#apidoc.element.inquirer.ui.BottomBar.prototype.updateBottomBar)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.BottomBar.prototype.</span>write (message)](#apidoc.element.inquirer.ui.BottomBar.prototype.write)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.BottomBar.prototype.</span>writeLog (data)](#apidoc.element.inquirer.ui.BottomBar.prototype.writeLog)

#### [module inquirer.ui.BottomBar.super_.prototype](#apidoc.module.inquirer.ui.BottomBar.super_.prototype)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.BottomBar.super_.prototype.</span>close ()](#apidoc.element.inquirer.ui.BottomBar.super_.prototype.close)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.BottomBar.super_.prototype.</span>onForceClose ()](#apidoc.element.inquirer.ui.BottomBar.super_.prototype.onForceClose)

#### [module inquirer.ui.Prompt](#apidoc.module.inquirer.ui.Prompt)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.</span>Prompt (prompts, opt)](#apidoc.element.inquirer.ui.Prompt.Prompt)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.Prompt.</span>super_ (opt)](#apidoc.element.inquirer.ui.Prompt.super_)

#### [module inquirer.ui.Prompt.prototype](#apidoc.module.inquirer.ui.Prompt.prototype)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.Prompt.prototype.</span>fetchAnswer (question)](#apidoc.element.inquirer.ui.Prompt.prototype.fetchAnswer)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.Prompt.prototype.</span>filterIfRunnable (question)](#apidoc.element.inquirer.ui.Prompt.prototype.filterIfRunnable)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.Prompt.prototype.</span>onCompletion (answers)](#apidoc.element.inquirer.ui.Prompt.prototype.onCompletion)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.Prompt.prototype.</span>processQuestion (question)](#apidoc.element.inquirer.ui.Prompt.prototype.processQuestion)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.Prompt.prototype.</span>run (questions)](#apidoc.element.inquirer.ui.Prompt.prototype.run)
1.  [function <span class="apidocSignatureSpan">inquirer.ui.Prompt.prototype.</span>setDefaultType (question)](#apidoc.element.inquirer.ui.Prompt.prototype.setDefaultType)



# <a name="apidoc.module.inquirer"></a>[module inquirer](#apidoc.module.inquirer)

#### <a name="apidoc.element.inquirer.Separator"></a>[function <span class="apidocSignatureSpan">inquirer.</span>Separator (line)](#apidoc.element.inquirer.Separator)
- description and source-code
```javascript
Separator = function (line) {
  this.type = 'separator';
  this.line = chalk.dim(line || new Array(15).join(figures.line));
}
```
- example usage
```shell
...

### Separator
<a name="separator"></a>
A separator can be added to any 'choices' array:

'''
// In the question object
choices: [ "Choice A", new inquirer.Separator(), "choice B" ]

// Which'll be displayed this way
[?] What do you want to do?
> Order a pizza
  Make a reservation
  --------
  Ask opening hours
...
```

#### <a name="apidoc.element.inquirer.createPromptModule"></a>[function <span class="apidocSignatureSpan">inquirer.</span>createPromptModule (opt)](#apidoc.element.inquirer.createPromptModule)
- description and source-code
```javascript
createPromptModule = function (opt) {
  var promptModule = function (questions) {
    var ui = new inquirer.ui.Prompt(promptModule.prompts, opt);
    var promise = ui.run(questions);

    // Monkey patch the UI on the promise object so
    // that it remains publicly accessible.
    promise.ui = ui;

    return promise;
  };
  promptModule.prompts = {};

<span class="apidocCodeCommentSpan">  /**
   * Register a prompt type
   * @param {String} name     Prompt type name
   * @param {Function} prompt Prompt constructor
   * @return {inquirer}
   */
</span>
  promptModule.registerPrompt = function (name, prompt) {
    promptModule.prompts[name] = prompt;
    return this;
  };

  /**
   * Register the defaults provider prompts
   */

  promptModule.restoreDefaultPrompts = function () {
    this.registerPrompt('list', require('./prompts/list'));
    this.registerPrompt('input', require('./prompts/input'));
    this.registerPrompt('confirm', require('./prompts/confirm'));
    this.registerPrompt('rawlist', require('./prompts/rawlist'));
    this.registerPrompt('expand', require('./prompts/expand'));
    this.registerPrompt('checkbox', require('./prompts/checkbox'));
    this.registerPrompt('password', require('./prompts/password'));
    this.registerPrompt('editor', require('./prompts/editor'));
  };

  promptModule.restoreDefaultPrompts();

  return promptModule;
}
```
- example usage
```shell
...
#### 'inquirer.registerPrompt(name, prompt)'

Register prompt plugins under 'name'.

- **name** (string) name of the this new prompt. (used for question 'type')
- **prompt** (object) the prompt object itself (the plugin)

#### 'inquirer.createPromptModule() -> prompt function'

Create a self contained inquirer module. If don't want to affect other libraries that also rely on inquirer when you overwrite or
 add new prompt types.

'''js
var prompt = inquirer.createPromptModule();

prompt(questions).then(/* ... */);
...
```

#### <a name="apidoc.element.inquirer.prompt"></a>[function <span class="apidocSignatureSpan">inquirer.</span>prompt (questions)](#apidoc.element.inquirer.prompt)
- description and source-code
```javascript
prompt = function (questions) {
  var ui = new inquirer.ui.Prompt(promptModule.prompts, opt);
  var promise = ui.run(questions);

  // Monkey patch the UI on the promise object so
  // that it remains publicly accessible.
  promise.ui = ui;

  return promise;
}
```
- example usage
```shell
...

''' shell
npm install inquirer
'''

'''javascript
var inquirer = require('inquirer');
inquirer.prompt([/* Pass your questions in here */]).then(function (answers) {
	// Use user feedback for... whatever!!
});
'''

<a name="examples"></a>
### Examples (Run it and see it)
Check out the 'examples/' folder for code and interface examples.
...
```

#### <a name="apidoc.element.inquirer.registerPrompt"></a>[function <span class="apidocSignatureSpan">inquirer.</span>registerPrompt (name, prompt)](#apidoc.element.inquirer.registerPrompt)
- description and source-code
```javascript
registerPrompt = function (name, prompt) {
  inquirer.prompt.registerPrompt(name, prompt);
}
```
- example usage
```shell
...
#### 'inquirer.prompt(questions) -> promise'

Launch the prompt interface (inquiry session)

- **questions** (Array) containing [Question Object](#question) (using the [reactive interface](#reactive-interface), you can also
 pass a 'Rx.Observable' instance)
- returns a **Promise**

#### 'inquirer.registerPrompt(name, prompt)'

Register prompt plugins under 'name'.

- **name** (string) name of the this new prompt. (used for question 'type')
- **prompt** (object) the prompt object itself (the plugin)

#### 'inquirer.createPromptModule() -> prompt function'
...
```

#### <a name="apidoc.element.inquirer.restoreDefaultPrompts"></a>[function <span class="apidocSignatureSpan">inquirer.</span>restoreDefaultPrompts ()](#apidoc.element.inquirer.restoreDefaultPrompts)
- description and source-code
```javascript
restoreDefaultPrompts = function () {
  inquirer.prompt.restoreDefaultPrompts();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.ui.BottomBar"></a>[function <span class="apidocSignatureSpan">inquirer.</span>ui.BottomBar (opt)](#apidoc.element.inquirer.ui.BottomBar)
- description and source-code
```javascript
function Prompt(opt) {
  opt || (opt = {});

  Base.apply(this, arguments);

  this.log = through(this.writeLog.bind(this));
  this.bottomBar = opt.bottomBar || '';
  this.render();
}
```
- example usage
```shell
...
Along with the prompts, Inquirer offers some basic text UI.

#### Bottom Bar - 'inquirer.ui.BottomBar'

This UI present a fixed text at the bottom of a free text zone. This is useful to keep a message to the bottom of the screen while
 outputting command outputs on the higher section.

'''javascript
var ui = new inquirer.ui.BottomBar();

// pipe a Stream to the log zone
outputStream.pipe(ui.log);

// Or simply write output
ui.log.write('something just happened.');
ui.log.write('Almost over, standby!');
...
```

#### <a name="apidoc.element.inquirer.ui.Prompt"></a>[function <span class="apidocSignatureSpan">inquirer.</span>ui.Prompt (prompts, opt)](#apidoc.element.inquirer.ui.Prompt)
- description and source-code
```javascript
ui.Prompt = function (prompts, opt) {
  Base.call(this, opt);
  this.prompts = prompts;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.inquirer.Separator"></a>[module inquirer.Separator](#apidoc.module.inquirer.Separator)

#### <a name="apidoc.element.inquirer.Separator.Separator"></a>[function <span class="apidocSignatureSpan">inquirer.</span>Separator (line)](#apidoc.element.inquirer.Separator.Separator)
- description and source-code
```javascript
Separator = function (line) {
  this.type = 'separator';
  this.line = chalk.dim(line || new Array(15).join(figures.line));
}
```
- example usage
```shell
...

### Separator
<a name="separator"></a>
A separator can be added to any 'choices' array:

'''
// In the question object
choices: [ "Choice A", new inquirer.Separator(), "choice B" ]

// Which'll be displayed this way
[?] What do you want to do?
> Order a pizza
  Make a reservation
  --------
  Ask opening hours
...
```

#### <a name="apidoc.element.inquirer.Separator.exclude"></a>[function <span class="apidocSignatureSpan">inquirer.Separator.</span>exclude (obj)](#apidoc.element.inquirer.Separator.exclude)
- description and source-code
```javascript
exclude = function (obj) {
  return obj.type !== 'separator';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.inquirer.Separator.prototype"></a>[module inquirer.Separator.prototype](#apidoc.module.inquirer.Separator.prototype)

#### <a name="apidoc.element.inquirer.Separator.prototype.toString"></a>[function <span class="apidocSignatureSpan">inquirer.Separator.prototype.</span>toString ()](#apidoc.element.inquirer.Separator.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this.line;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.inquirer.prompt"></a>[module inquirer.prompt](#apidoc.module.inquirer.prompt)

#### <a name="apidoc.element.inquirer.prompt.prompt"></a>[function <span class="apidocSignatureSpan">inquirer.</span>prompt (questions)](#apidoc.element.inquirer.prompt.prompt)
- description and source-code
```javascript
prompt = function (questions) {
  var ui = new inquirer.ui.Prompt(promptModule.prompts, opt);
  var promise = ui.run(questions);

  // Monkey patch the UI on the promise object so
  // that it remains publicly accessible.
  promise.ui = ui;

  return promise;
}
```
- example usage
```shell
...

''' shell
npm install inquirer
'''

'''javascript
var inquirer = require('inquirer');
inquirer.prompt([/* Pass your questions in here */]).then(function (answers) {
	// Use user feedback for... whatever!!
});
'''

<a name="examples"></a>
### Examples (Run it and see it)
Check out the 'examples/' folder for code and interface examples.
...
```

#### <a name="apidoc.element.inquirer.prompt.registerPrompt"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.</span>registerPrompt (name, prompt)](#apidoc.element.inquirer.prompt.registerPrompt)
- description and source-code
```javascript
registerPrompt = function (name, prompt) {
  promptModule.prompts[name] = prompt;
  return this;
}
```
- example usage
```shell
...
#### 'inquirer.prompt(questions) -> promise'

Launch the prompt interface (inquiry session)

- **questions** (Array) containing [Question Object](#question) (using the [reactive interface](#reactive-interface), you can also
 pass a 'Rx.Observable' instance)
- returns a **Promise**

#### 'inquirer.registerPrompt(name, prompt)'

Register prompt plugins under 'name'.

- **name** (string) name of the this new prompt. (used for question 'type')
- **prompt** (object) the prompt object itself (the plugin)

#### 'inquirer.createPromptModule() -> prompt function'
...
```

#### <a name="apidoc.element.inquirer.prompt.restoreDefaultPrompts"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.</span>restoreDefaultPrompts ()](#apidoc.element.inquirer.prompt.restoreDefaultPrompts)
- description and source-code
```javascript
restoreDefaultPrompts = function () {
  this.registerPrompt('list', require('./prompts/list'));
  this.registerPrompt('input', require('./prompts/input'));
  this.registerPrompt('confirm', require('./prompts/confirm'));
  this.registerPrompt('rawlist', require('./prompts/rawlist'));
  this.registerPrompt('expand', require('./prompts/expand'));
  this.registerPrompt('checkbox', require('./prompts/checkbox'));
  this.registerPrompt('password', require('./prompts/password'));
  this.registerPrompt('editor', require('./prompts/editor'));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.inquirer.prompt.prompts"></a>[module inquirer.prompt.prompts](#apidoc.module.inquirer.prompt.prompts)

#### <a name="apidoc.element.inquirer.prompt.prompts.checkbox"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.</span>checkbox ()](#apidoc.element.inquirer.prompt.prompts.checkbox)
- description and source-code
```javascript
function Prompt() {
  Base.apply(this, arguments);

  if (!this.opt.choices) {
    this.throwParamError('choices');
  }

  if (_.isArray(this.opt.default)) {
    this.opt.choices.forEach(function (choice) {
      if (this.opt.default.indexOf(choice.value) >= 0) {
        choice.checked = true;
      }
    }, this);
  }

  this.pointer = 0;
  this.firstRender = true;

  // Make sure no default is set (so it won't be printed)
  this.opt.default = null;

  this.paginator = new Paginator();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.confirm"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.</span>confirm ()](#apidoc.element.inquirer.prompt.prompts.confirm)
- description and source-code
```javascript
function Prompt() {
  Base.apply(this, arguments);

  var rawDefault = true;

  _.extend(this.opt, {
    filter: function (input) {
      var value = rawDefault;
      if (input != null && input !== '') {
        value = /^y(es)?/i.test(input);
      }
      return value;
    }
  });

  if (_.isBoolean(this.opt.default)) {
    rawDefault = this.opt.default;
  }

  this.opt.default = rawDefault ? 'Y/n' : 'y/N';

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.editor"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.</span>editor ()](#apidoc.element.inquirer.prompt.prompts.editor)
- description and source-code
```javascript
function Prompt() {
  return Base.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.expand"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.</span>expand ()](#apidoc.element.inquirer.prompt.prompts.expand)
- description and source-code
```javascript
function Prompt() {
  Base.apply(this, arguments);

  if (!this.opt.choices) {
    this.throwParamError('choices');
  }

  this.validateChoices(this.opt.choices);

  // Add the default 'help' (/expand) option
  this.opt.choices.push({
    key: 'h',
    name: 'Help, list all options',
    value: 'help'
  });

  this.opt.validate = function (choice) {
    if (choice == null) {
      return 'Please enter a valid command';
    }

    return choice !== 'help';
  };

  // Setup the default string (capitalize the default key)
  this.opt.default = this.generateChoicesString(this.opt.choices, this.opt.default);

  this.paginator = new Paginator();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.input"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.</span>input ()](#apidoc.element.inquirer.prompt.prompts.input)
- description and source-code
```javascript
function Prompt() {
  return Base.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.list"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.</span>list ()](#apidoc.element.inquirer.prompt.prompts.list)
- description and source-code
```javascript
function Prompt() {
  Base.apply(this, arguments);

  if (!this.opt.choices) {
    this.throwParamError('choices');
  }

  this.firstRender = true;
  this.selected = 0;

  var def = this.opt.default;

  // Default being a Number
  if (_.isNumber(def) && def >= 0 && def < this.opt.choices.realLength) {
    this.selected = def;
  }

  // Default being a String
  if (_.isString(def)) {
    this.selected = this.opt.choices.pluck('value').indexOf(def);
  }

  // Make sure no default is set (so it won't be printed)
  this.opt.default = null;

  this.paginator = new Paginator();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.password"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.</span>password ()](#apidoc.element.inquirer.prompt.prompts.password)
- description and source-code
```javascript
function Prompt() {
  return Base.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.rawlist"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.</span>rawlist ()](#apidoc.element.inquirer.prompt.prompts.rawlist)
- description and source-code
```javascript
function Prompt() {
  Base.apply(this, arguments);

  if (!this.opt.choices) {
    this.throwParamError('choices');
  }

  this.opt.validChoices = this.opt.choices.filter(Separator.exclude);

  this.selected = 0;
  this.rawDefault = 0;

  _.extend(this.opt, {
    validate: function (val) {
      return val != null;
    }
  });

  var def = this.opt.default;
  if (_.isNumber(def) && def >= 0 && def < this.opt.choices.realLength) {
    this.selected = this.rawDefault = def;
  }

  // Make sure no default is set (so it won't be printed)
  this.opt.default = null;

  this.paginator = new Paginator();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.inquirer.prompt.prompts.checkbox.prototype"></a>[module inquirer.prompt.prompts.checkbox.prototype](#apidoc.module.inquirer.prompt.prompts.checkbox.prototype)

#### <a name="apidoc.element.inquirer.prompt.prompts.checkbox.prototype._run"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>_run (cb)](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype._run)
- description and source-code
```javascript
_run = function (cb) {
  this.done = cb;

  var events = observe(this.rl);

  var validation = this.handleSubmitEvents(
    events.line.map(this.getCurrentValue.bind(this))
  );
  validation.success.forEach(this.onEnd.bind(this));
  validation.error.forEach(this.onError.bind(this));

  events.normalizedUpKey.takeUntil(validation.success).forEach(this.onUpKey.bind(this));
  events.normalizedDownKey.takeUntil(validation.success).forEach(this.onDownKey.bind(this));
  events.numberKey.takeUntil(validation.success).forEach(this.onNumberKey.bind(this));
  events.spaceKey.takeUntil(validation.success).forEach(this.onSpaceKey.bind(this));
  events.aKey.takeUntil(validation.success).forEach(this.onAllKey.bind(this));
  events.iKey.takeUntil(validation.success).forEach(this.onInverseKey.bind(this));

  // Init the prompt
  cliCursor.hide();
  this.render();
  this.firstRender = false;

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.checkbox.prototype.getCurrentValue"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>getCurrentValue ()](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.getCurrentValue)
- description and source-code
```javascript
getCurrentValue = function () {
  var choices = this.opt.choices.filter(function (choice) {
    return Boolean(choice.checked) && !choice.disabled;
  });

  this.selection = _.map(choices, 'short');
  return _.map(choices, 'value');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onAllKey"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>onAllKey ()](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onAllKey)
- description and source-code
```javascript
onAllKey = function () {
  var shouldBeChecked = Boolean(this.opt.choices.find(function (choice) {
    return choice.type !== 'separator' && !choice.checked;
  }));

  this.opt.choices.forEach(function (choice) {
    if (choice.type !== 'separator') {
      choice.checked = shouldBeChecked;
    }
  });

  this.render();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onDownKey"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>onDownKey ()](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onDownKey)
- description and source-code
```javascript
onDownKey = function () {
  var len = this.opt.choices.realLength;
  this.pointer = (this.pointer < len - 1) ? this.pointer + 1 : 0;
  this.render();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onEnd"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>onEnd (state)](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onEnd)
- description and source-code
```javascript
onEnd = function (state) {
  this.status = 'answered';

  // Rerender prompt (and clean subline error)
  this.render();

  this.screen.done();
  cliCursor.show();
  this.done(state.value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onError"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>onError (state)](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onError)
- description and source-code
```javascript
onError = function (state) {
  this.render(state.isValid);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onInverseKey"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>onInverseKey ()](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onInverseKey)
- description and source-code
```javascript
onInverseKey = function () {
  this.opt.choices.forEach(function (choice) {
    if (choice.type !== 'separator') {
      choice.checked = !choice.checked;
    }
  });

  this.render();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onNumberKey"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>onNumberKey (input)](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onNumberKey)
- description and source-code
```javascript
onNumberKey = function (input) {
  if (input <= this.opt.choices.realLength) {
    this.pointer = input - 1;
    this.toggleChoice(this.pointer);
  }
  this.render();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onSpaceKey"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>onSpaceKey ()](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onSpaceKey)
- description and source-code
```javascript
onSpaceKey = function () {
  this.toggleChoice(this.pointer);
  this.render();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onUpKey"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>onUpKey ()](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.onUpKey)
- description and source-code
```javascript
onUpKey = function () {
  var len = this.opt.choices.realLength;
  this.pointer = (this.pointer > 0) ? this.pointer - 1 : len - 1;
  this.render();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.checkbox.prototype.render"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>render (error)](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.render)
- description and source-code
```javascript
render = function (error) {
  // Render question
  var message = this.getQuestion();
  var bottomContent = '';

  if (this.firstRender) {
    message += '(Press ' + chalk.cyan.bold('<space>') + ' to select, ' + chalk.cyan.bold('<a>') + ' to toggle all, ' + chalk.cyan
.bold('<i>') + ' to inverse selection)';
  }

  // Render choices or answer depending on the state
  if (this.status === 'answered') {
    message += chalk.cyan(this.selection.join(', '));
  } else {
    var choicesStr = renderChoices(this.opt.choices, this.pointer);
    var indexPosition = this.opt.choices.indexOf(this.opt.choices.getChoice(this.pointer));
    message += '\n' + this.paginator.paginate(choicesStr, indexPosition, this.opt.pageSize);
  }

  if (error) {
    bottomContent = chalk.red('>> ') + error;
  }

  this.screen.render(message, bottomContent);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.checkbox.prototype.toggleChoice"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.checkbox.prototype.</span>toggleChoice (index)](#apidoc.element.inquirer.prompt.prompts.checkbox.prototype.toggleChoice)
- description and source-code
```javascript
toggleChoice = function (index) {
  var item = this.opt.choices.getChoice(index);
  if (item !== undefined) {
    this.opt.choices.getChoice(index).checked = !item.checked;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.inquirer.prompt.prompts.confirm.prototype"></a>[module inquirer.prompt.prompts.confirm.prototype](#apidoc.module.inquirer.prompt.prompts.confirm.prototype)

#### <a name="apidoc.element.inquirer.prompt.prompts.confirm.prototype._run"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.confirm.prototype.</span>_run (cb)](#apidoc.element.inquirer.prompt.prompts.confirm.prototype._run)
- description and source-code
```javascript
_run = function (cb) {
  this.done = cb;

  // Once user confirm (enter key)
  var events = observe(this.rl);
  events.keypress.takeUntil(events.line).forEach(this.onKeypress.bind(this));

  events.line.take(1).forEach(this.onEnd.bind(this));

  // Init
  this.render();

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.confirm.prototype.onEnd"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.confirm.prototype.</span>onEnd (input)](#apidoc.element.inquirer.prompt.prompts.confirm.prototype.onEnd)
- description and source-code
```javascript
onEnd = function (input) {
  this.status = 'answered';

  var output = this.opt.filter(input);
  this.render(output);

  this.screen.done();
  this.done(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.confirm.prototype.onKeypress"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.confirm.prototype.</span>onKeypress ()](#apidoc.element.inquirer.prompt.prompts.confirm.prototype.onKeypress)
- description and source-code
```javascript
onKeypress = function () {
  this.render();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.confirm.prototype.render"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.confirm.prototype.</span>render (answer)](#apidoc.element.inquirer.prompt.prompts.confirm.prototype.render)
- description and source-code
```javascript
render = function (answer) {
  var message = this.getQuestion();

  if (typeof answer === 'boolean') {
    message += chalk.cyan(answer ? 'Yes' : 'No');
  } else {
    message += this.rl.line;
  }

  this.screen.render(message);

  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.inquirer.prompt.prompts.editor.prototype"></a>[module inquirer.prompt.prompts.editor.prototype](#apidoc.module.inquirer.prompt.prompts.editor.prototype)

#### <a name="apidoc.element.inquirer.prompt.prompts.editor.prototype._run"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.editor.prototype.</span>_run (cb)](#apidoc.element.inquirer.prompt.prompts.editor.prototype._run)
- description and source-code
```javascript
_run = function (cb) {
  this.done = cb;

  this.editorResult = new rx.Subject();

  // Open Editor on "line" (Enter Key)
  var events = observe(this.rl);
  this.lineSubscription = events.line.forEach(this.startExternalEditor.bind(this));

  // Trigger Validation when editor closes
  var validation = this.handleSubmitEvents(this.editorResult);
  validation.success.forEach(this.onEnd.bind(this));
  validation.error.forEach(this.onError.bind(this));

  // Prevents default from being printed on screen (can look weird with multiple lines)
  this.currentText = this.opt.default;
  this.opt.default = null;

  // Init
  this.render();

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.editor.prototype.endExternalEditor"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.editor.prototype.</span>endExternalEditor (error, result)](#apidoc.element.inquirer.prompt.prompts.editor.prototype.endExternalEditor)
- description and source-code
```javascript
endExternalEditor = function (error, result) {
  this.rl.resume();
  if (error) {
    this.editorResult.onError(error);
  } else {
    this.editorResult.onNext(result);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.editor.prototype.onEnd"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.editor.prototype.</span>onEnd (state)](#apidoc.element.inquirer.prompt.prompts.editor.prototype.onEnd)
- description and source-code
```javascript
onEnd = function (state) {
  this.editorResult.dispose();
  this.lineSubscription.dispose();
  this.answer = state.value;
  this.status = 'answered';
  // Re-render prompt
  this.render();
  this.screen.done();
  this.done(this.answer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.editor.prototype.onError"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.editor.prototype.</span>onError (state)](#apidoc.element.inquirer.prompt.prompts.editor.prototype.onError)
- description and source-code
```javascript
onError = function (state) {
  this.render(state.isValid);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.editor.prototype.render"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.editor.prototype.</span>render (error)](#apidoc.element.inquirer.prompt.prompts.editor.prototype.render)
- description and source-code
```javascript
render = function (error) {
  var bottomContent = '';
  var message = this.getQuestion();

  if (this.status === 'answered') {
    message += chalk.dim('Received');
  } else {
    message += chalk.dim('Press <enter> to launch your preferred editor.');
  }

  if (error) {
    bottomContent = chalk.red('>> ') + error;
  }

  this.screen.render(message, bottomContent);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.editor.prototype.startExternalEditor"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.editor.prototype.</span>startExternalEditor ()](#apidoc.element.inquirer.prompt.prompts.editor.prototype.startExternalEditor)
- description and source-code
```javascript
startExternalEditor = function () {
  // Pause Readline to prevent stdin and stdout from being modified while the editor is showing
  this.rl.pause();
  ExternalEditor.editAsync(this.currentText, this.endExternalEditor.bind(this));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.inquirer.prompt.prompts.expand.prototype"></a>[module inquirer.prompt.prompts.expand.prototype](#apidoc.module.inquirer.prompt.prompts.expand.prototype)

#### <a name="apidoc.element.inquirer.prompt.prompts.expand.prototype._run"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.expand.prototype.</span>_run (cb)](#apidoc.element.inquirer.prompt.prompts.expand.prototype._run)
- description and source-code
```javascript
_run = function (cb) {
  this.done = cb;

  // Save user answer and update prompt to show selected option.
  var events = observe(this.rl);
  var validation = this.handleSubmitEvents(
    events.line.map(this.getCurrentValue.bind(this))
  );
  validation.success.forEach(this.onSubmit.bind(this));
  validation.error.forEach(this.onError.bind(this));
  this.keypressObs = events.keypress.takeUntil(validation.success)
    .forEach(this.onKeypress.bind(this));

  // Init the prompt
  this.render();

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.expand.prototype.generateChoicesString"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.expand.prototype.</span>generateChoicesString (choices, defaultIndex)](#apidoc.element.inquirer.prompt.prompts.expand.prototype.generateChoicesString)
- description and source-code
```javascript
generateChoicesString = function (choices, defaultIndex) {
  var defIndex = choices.realLength - 1;
  if (_.isNumber(defaultIndex) && this.opt.choices.getChoice(defaultIndex)) {
    defIndex = defaultIndex;
  }
  var defStr = this.opt.choices.pluck('key');
  this.rawDefault = defStr[defIndex];
  defStr[defIndex] = String(defStr[defIndex]).toUpperCase();
  return defStr.join('');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.expand.prototype.getChoices"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.expand.prototype.</span>getChoices ()](#apidoc.element.inquirer.prompt.prompts.expand.prototype.getChoices)
- description and source-code
```javascript
getChoices = function () {
  var output = '';

  this.opt.choices.forEach(function (choice) {
    output += '\n  ';

    if (choice.type === 'separator') {
      output += ' ' + choice;
      return;
    }

    var choiceStr = choice.key + ') ' + choice.name;
    if (this.selectedKey === choice.key) {
      choiceStr = chalk.cyan(choiceStr);
    }
    output += choiceStr;
  }.bind(this));

  return output;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.expand.prototype.getCurrentValue"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.expand.prototype.</span>getCurrentValue (input)](#apidoc.element.inquirer.prompt.prompts.expand.prototype.getCurrentValue)
- description and source-code
```javascript
getCurrentValue = function (input) {
  if (!input) {
    input = this.rawDefault;
  }
  var selected = this.opt.choices.where({key: input.toLowerCase().trim()})[0];
  if (!selected) {
    return null;
  }

  return selected.value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.expand.prototype.onError"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.expand.prototype.</span>onError (state)](#apidoc.element.inquirer.prompt.prompts.expand.prototype.onError)
- description and source-code
```javascript
onError = function (state) {
  if (state.value === 'help') {
    this.selectedKey = '';
    this.status = 'expanded';
    this.render();
    return;
  }
  this.render(state.isValid);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.expand.prototype.onKeypress"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.expand.prototype.</span>onKeypress ()](#apidoc.element.inquirer.prompt.prompts.expand.prototype.onKeypress)
- description and source-code
```javascript
onKeypress = function () {
  this.selectedKey = this.rl.line.toLowerCase();
  var selected = this.opt.choices.where({key: this.selectedKey})[0];
  if (this.status === 'expanded') {
    this.render();
  } else {
    this.render(null, selected ? selected.name : null);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.expand.prototype.onSubmit"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.expand.prototype.</span>onSubmit (state)](#apidoc.element.inquirer.prompt.prompts.expand.prototype.onSubmit)
- description and source-code
```javascript
onSubmit = function (state) {
  this.status = 'answered';
  var choice = this.opt.choices.where({value: state.value})[0];
  this.answer = choice.short || choice.name;

  // Re-render prompt
  this.render();
  this.screen.done();
  this.done(state.value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.expand.prototype.render"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.expand.prototype.</span>render (error, hint)](#apidoc.element.inquirer.prompt.prompts.expand.prototype.render)
- description and source-code
```javascript
render = function (error, hint) {
  var message = this.getQuestion();
  var bottomContent = '';

  if (this.status === 'answered') {
    message += chalk.cyan(this.answer);
  } else if (this.status === 'expanded') {
    var choicesStr = renderChoices(this.opt.choices, this.selectedKey);
    message += this.paginator.paginate(choicesStr, this.selectedKey, this.opt.pageSize);
    message += '\n  Answer: ';
  }

  message += this.rl.line;

  if (error) {
    bottomContent = chalk.red('>> ') + error;
  }

  if (hint) {
    bottomContent = chalk.cyan('>> ') + hint;
  }

  this.screen.render(message, bottomContent);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.expand.prototype.validateChoices"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.expand.prototype.</span>validateChoices (choices)](#apidoc.element.inquirer.prompt.prompts.expand.prototype.validateChoices)
- description and source-code
```javascript
validateChoices = function (choices) {
  var formatError;
  var errors = [];
  var keymap = {};
  choices.filter(Separator.exclude).forEach(function (choice) {
    if (!choice.key || choice.key.length !== 1) {
      formatError = true;
    }
    if (keymap[choice.key]) {
      errors.push(choice.key);
    }
    keymap[choice.key] = true;
    choice.key = String(choice.key).toLowerCase();
  });

  if (formatError) {
    throw new Error('Format error: 'key' param must be a single letter and is required.');
  }
  if (keymap.h) {
    throw new Error('Reserved key error: 'key' param cannot be 'h' - this value is reserved.');
  }
  if (errors.length) {
    throw new Error('Duplicate key error: 'key' param must be unique. Duplicates: ' +
        _.uniq(errors).join(', '));
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.inquirer.prompt.prompts.input.prototype"></a>[module inquirer.prompt.prompts.input.prototype](#apidoc.module.inquirer.prompt.prompts.input.prototype)

#### <a name="apidoc.element.inquirer.prompt.prompts.input.prototype._run"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.input.prototype.</span>_run (cb)](#apidoc.element.inquirer.prompt.prompts.input.prototype._run)
- description and source-code
```javascript
_run = function (cb) {
  this.done = cb;

  // Once user confirm (enter key)
  var events = observe(this.rl);
  var submit = events.line.map(this.filterInput.bind(this));

  var validation = this.handleSubmitEvents(submit);
  validation.success.forEach(this.onEnd.bind(this));
  validation.error.forEach(this.onError.bind(this));

  events.keypress.takeUntil(validation.success).forEach(this.onKeypress.bind(this));

  // Init
  this.render();

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.input.prototype.filterInput"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.input.prototype.</span>filterInput (input)](#apidoc.element.inquirer.prompt.prompts.input.prototype.filterInput)
- description and source-code
```javascript
filterInput = function (input) {
  if (!input) {
    return this.opt.default == null ? '' : this.opt.default;
  }
  return input;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.input.prototype.onEnd"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.input.prototype.</span>onEnd (state)](#apidoc.element.inquirer.prompt.prompts.input.prototype.onEnd)
- description and source-code
```javascript
onEnd = function (state) {
  this.answer = state.value;
  this.status = 'answered';

  // Re-render prompt
  this.render();

  this.screen.done();
  this.done(state.value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.input.prototype.onError"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.input.prototype.</span>onError (state)](#apidoc.element.inquirer.prompt.prompts.input.prototype.onError)
- description and source-code
```javascript
onError = function (state) {
  this.render(state.isValid);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.input.prototype.onKeypress"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.input.prototype.</span>onKeypress ()](#apidoc.element.inquirer.prompt.prompts.input.prototype.onKeypress)
- description and source-code
```javascript
onKeypress = function () {
  this.render();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.input.prototype.render"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.input.prototype.</span>render (error)](#apidoc.element.inquirer.prompt.prompts.input.prototype.render)
- description and source-code
```javascript
render = function (error) {
  var bottomContent = '';
  var message = this.getQuestion();

  if (this.status === 'answered') {
    message += chalk.cyan(this.answer);
  } else {
    message += this.rl.line;
  }

  if (error) {
    bottomContent = chalk.red('>> ') + error;
  }

  this.screen.render(message, bottomContent);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.inquirer.prompt.prompts.list.prototype"></a>[module inquirer.prompt.prompts.list.prototype](#apidoc.module.inquirer.prompt.prompts.list.prototype)

#### <a name="apidoc.element.inquirer.prompt.prompts.list.prototype._run"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.list.prototype.</span>_run (cb)](#apidoc.element.inquirer.prompt.prompts.list.prototype._run)
- description and source-code
```javascript
_run = function (cb) {
  this.done = cb;

  var self = this;

  var events = observe(this.rl);
  events.normalizedUpKey.takeUntil(events.line).forEach(this.onUpKey.bind(this));
  events.normalizedDownKey.takeUntil(events.line).forEach(this.onDownKey.bind(this));
  events.numberKey.takeUntil(events.line).forEach(this.onNumberKey.bind(this));
  events.line
    .take(1)
    .map(this.getCurrentValue.bind(this))
    .flatMap(function (value) {
      return runAsync(self.opt.filter)(value).catch(function (err) {
        return err;
      });
    })
    .forEach(this.onSubmit.bind(this));

  // Init the prompt
  cliCursor.hide();
  this.render();

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.list.prototype.getCurrentValue"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.list.prototype.</span>getCurrentValue ()](#apidoc.element.inquirer.prompt.prompts.list.prototype.getCurrentValue)
- description and source-code
```javascript
getCurrentValue = function () {
  return this.opt.choices.getChoice(this.selected).value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.list.prototype.onDownKey"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.list.prototype.</span>onDownKey ()](#apidoc.element.inquirer.prompt.prompts.list.prototype.onDownKey)
- description and source-code
```javascript
onDownKey = function () {
  var len = this.opt.choices.realLength;
  this.selected = (this.selected < len - 1) ? this.selected + 1 : 0;
  this.render();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.list.prototype.onNumberKey"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.list.prototype.</span>onNumberKey (input)](#apidoc.element.inquirer.prompt.prompts.list.prototype.onNumberKey)
- description and source-code
```javascript
onNumberKey = function (input) {
  if (input <= this.opt.choices.realLength) {
    this.selected = input - 1;
  }
  this.render();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.list.prototype.onSubmit"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.list.prototype.</span>onSubmit (value)](#apidoc.element.inquirer.prompt.prompts.list.prototype.onSubmit)
- description and source-code
```javascript
onSubmit = function (value) {
  this.status = 'answered';

  // Rerender prompt
  this.render();

  this.screen.done();
  cliCursor.show();
  this.done(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.list.prototype.onUpKey"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.list.prototype.</span>onUpKey ()](#apidoc.element.inquirer.prompt.prompts.list.prototype.onUpKey)
- description and source-code
```javascript
onUpKey = function () {
  var len = this.opt.choices.realLength;
  this.selected = (this.selected > 0) ? this.selected - 1 : len - 1;
  this.render();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.list.prototype.render"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.list.prototype.</span>render ()](#apidoc.element.inquirer.prompt.prompts.list.prototype.render)
- description and source-code
```javascript
render = function () {
  // Render question
  var message = this.getQuestion();

  if (this.firstRender) {
    message += chalk.dim('(Use arrow keys)');
  }

  // Render choices or answer depending on the state
  if (this.status === 'answered') {
    message += chalk.cyan(this.opt.choices.getChoice(this.selected).short);
  } else {
    var choicesStr = listRender(this.opt.choices, this.selected);
    var indexPosition = this.opt.choices.indexOf(this.opt.choices.getChoice(this.selected));
    message += '\n' + this.paginator.paginate(choicesStr, indexPosition, this.opt.pageSize);
  }

  this.firstRender = false;

  this.screen.render(message);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.inquirer.prompt.prompts.password.prototype"></a>[module inquirer.prompt.prompts.password.prototype](#apidoc.module.inquirer.prompt.prompts.password.prototype)

#### <a name="apidoc.element.inquirer.prompt.prompts.password.prototype._run"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.password.prototype.</span>_run (cb)](#apidoc.element.inquirer.prompt.prompts.password.prototype._run)
- description and source-code
```javascript
_run = function (cb) {
  this.done = cb;

  var events = observe(this.rl);

  // Once user confirm (enter key)
  var submit = events.line.map(this.filterInput.bind(this));

  var validation = this.handleSubmitEvents(submit);
  validation.success.forEach(this.onEnd.bind(this));
  validation.error.forEach(this.onError.bind(this));

  events.keypress.takeUntil(validation.success).forEach(this.onKeypress.bind(this));

  // Init
  this.render();

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.password.prototype.filterInput"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.password.prototype.</span>filterInput (input)](#apidoc.element.inquirer.prompt.prompts.password.prototype.filterInput)
- description and source-code
```javascript
filterInput = function (input) {
  if (!input) {
    return this.opt.default == null ? '' : this.opt.default;
  }
  return input;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.password.prototype.onEnd"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.password.prototype.</span>onEnd (state)](#apidoc.element.inquirer.prompt.prompts.password.prototype.onEnd)
- description and source-code
```javascript
onEnd = function (state) {
  this.status = 'answered';
  this.answer = state.value;

  // Re-render prompt
  this.render();

  this.screen.done();
  this.done(state.value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.password.prototype.onError"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.password.prototype.</span>onError (state)](#apidoc.element.inquirer.prompt.prompts.password.prototype.onError)
- description and source-code
```javascript
onError = function (state) {
  this.render(state.isValid);
  this.rl.output.unmute();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.password.prototype.onKeypress"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.password.prototype.</span>onKeypress ()](#apidoc.element.inquirer.prompt.prompts.password.prototype.onKeypress)
- description and source-code
```javascript
onKeypress = function () {
  this.render();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.password.prototype.render"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.password.prototype.</span>render (error)](#apidoc.element.inquirer.prompt.prompts.password.prototype.render)
- description and source-code
```javascript
render = function (error) {
  var message = this.getQuestion();
  var bottomContent = '';

  if (this.status === 'answered') {
    message += chalk.cyan(mask(this.answer));
  } else {
    message += mask(this.rl.line || '');
  }

  if (error) {
    bottomContent = '\n' + chalk.red('>> ') + error;
  }

  this.screen.render(message, bottomContent);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.inquirer.prompt.prompts.rawlist.prototype"></a>[module inquirer.prompt.prompts.rawlist.prototype](#apidoc.module.inquirer.prompt.prompts.rawlist.prototype)

#### <a name="apidoc.element.inquirer.prompt.prompts.rawlist.prototype._run"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.rawlist.prototype.</span>_run (cb)](#apidoc.element.inquirer.prompt.prompts.rawlist.prototype._run)
- description and source-code
```javascript
_run = function (cb) {
  this.done = cb;

  // Once user confirm (enter key)
  var events = observe(this.rl);
  var submit = events.line.map(this.getCurrentValue.bind(this));

  var validation = this.handleSubmitEvents(submit);
  validation.success.forEach(this.onEnd.bind(this));
  validation.error.forEach(this.onError.bind(this));

  events.keypress.takeUntil(validation.success).forEach(this.onKeypress.bind(this));

  // Init the prompt
  this.render();

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.rawlist.prototype.getCurrentValue"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.rawlist.prototype.</span>getCurrentValue (index)](#apidoc.element.inquirer.prompt.prompts.rawlist.prototype.getCurrentValue)
- description and source-code
```javascript
getCurrentValue = function (index) {
  if (index == null || index === '') {
    index = this.rawDefault;
  } else {
    index -= 1;
  }

  var choice = this.opt.choices.getChoice(index);
  return choice ? choice.value : null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.rawlist.prototype.onEnd"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.rawlist.prototype.</span>onEnd (state)](#apidoc.element.inquirer.prompt.prompts.rawlist.prototype.onEnd)
- description and source-code
```javascript
onEnd = function (state) {
  this.status = 'answered';
  this.answer = state.value;

  // Re-render prompt
  this.render();

  this.screen.done();
  this.done(state.value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.rawlist.prototype.onError"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.rawlist.prototype.</span>onError ()](#apidoc.element.inquirer.prompt.prompts.rawlist.prototype.onError)
- description and source-code
```javascript
onError = function () {
  this.render('Please enter a valid index');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.rawlist.prototype.onKeypress"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.rawlist.prototype.</span>onKeypress ()](#apidoc.element.inquirer.prompt.prompts.rawlist.prototype.onKeypress)
- description and source-code
```javascript
onKeypress = function () {
  var index = this.rl.line.length ? Number(this.rl.line) - 1 : 0;

  if (this.opt.choices.getChoice(index)) {
    this.selected = index;
  } else {
    this.selected = undefined;
  }

  this.render();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.prompt.prompts.rawlist.prototype.render"></a>[function <span class="apidocSignatureSpan">inquirer.prompt.prompts.rawlist.prototype.</span>render (error)](#apidoc.element.inquirer.prompt.prompts.rawlist.prototype.render)
- description and source-code
```javascript
render = function (error) {
  // Render question
  var message = this.getQuestion();
  var bottomContent = '';

  if (this.status === 'answered') {
    message += chalk.cyan(this.answer);
  } else {
    var choicesStr = renderChoices(this.opt.choices, this.selected);
    message += this.paginator.paginate(choicesStr, this.selected, this.opt.pageSize);
    message += '\n  Answer: ';
  }

  message += this.rl.line;

  if (error) {
    bottomContent = '\n' + chalk.red('>> ') + error;
  }

  this.screen.render(message, bottomContent);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.inquirer.ui"></a>[module inquirer.ui](#apidoc.module.inquirer.ui)

#### <a name="apidoc.element.inquirer.ui.BottomBar"></a>[function <span class="apidocSignatureSpan">inquirer.ui.</span>BottomBar (opt)](#apidoc.element.inquirer.ui.BottomBar)
- description and source-code
```javascript
function Prompt(opt) {
  opt || (opt = {});

  Base.apply(this, arguments);

  this.log = through(this.writeLog.bind(this));
  this.bottomBar = opt.bottomBar || '';
  this.render();
}
```
- example usage
```shell
...
Along with the prompts, Inquirer offers some basic text UI.

#### Bottom Bar - 'inquirer.ui.BottomBar'

This UI present a fixed text at the bottom of a free text zone. This is useful to keep a message to the bottom of the screen while
 outputting command outputs on the higher section.

'''javascript
var ui = new inquirer.ui.BottomBar();

// pipe a Stream to the log zone
outputStream.pipe(ui.log);

// Or simply write output
ui.log.write('something just happened.');
ui.log.write('Almost over, standby!');
...
```

#### <a name="apidoc.element.inquirer.ui.Prompt"></a>[function <span class="apidocSignatureSpan">inquirer.ui.</span>Prompt (prompts, opt)](#apidoc.element.inquirer.ui.Prompt)
- description and source-code
```javascript
Prompt = function (prompts, opt) {
  Base.call(this, opt);
  this.prompts = prompts;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.inquirer.ui.BottomBar"></a>[module inquirer.ui.BottomBar](#apidoc.module.inquirer.ui.BottomBar)

#### <a name="apidoc.element.inquirer.ui.BottomBar.BottomBar"></a>[function <span class="apidocSignatureSpan">inquirer.ui.</span>BottomBar (opt)](#apidoc.element.inquirer.ui.BottomBar.BottomBar)
- description and source-code
```javascript
function Prompt(opt) {
  opt || (opt = {});

  Base.apply(this, arguments);

  this.log = through(this.writeLog.bind(this));
  this.bottomBar = opt.bottomBar || '';
  this.render();
}
```
- example usage
```shell
...
Along with the prompts, Inquirer offers some basic text UI.

#### Bottom Bar - 'inquirer.ui.BottomBar'

This UI present a fixed text at the bottom of a free text zone. This is useful to keep a message to the bottom of the screen while
 outputting command outputs on the higher section.

'''javascript
var ui = new inquirer.ui.BottomBar();

// pipe a Stream to the log zone
outputStream.pipe(ui.log);

// Or simply write output
ui.log.write('something just happened.');
ui.log.write('Almost over, standby!');
...
```

#### <a name="apidoc.element.inquirer.ui.BottomBar.super_"></a>[function <span class="apidocSignatureSpan">inquirer.ui.BottomBar.</span>super_ (opt)](#apidoc.element.inquirer.ui.BottomBar.super_)
- description and source-code
```javascript
super_ = function (opt) {
  // Instantiate the Readline interface
  // @Note: Don't reassign if already present (allow test to override the Stream)
  if (!this.rl) {
    this.rl = readline.createInterface(setupReadlineOptions(opt));
  }
  this.rl.resume();

  this.onForceClose = this.onForceClose.bind(this);

  // Make sure new prompt start on a newline when closing
  this.rl.on('SIGINT', this.onForceClose);
  process.on('exit', this.onForceClose);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.inquirer.ui.BottomBar.prototype"></a>[module inquirer.ui.BottomBar.prototype](#apidoc.module.inquirer.ui.BottomBar.prototype)

#### <a name="apidoc.element.inquirer.ui.BottomBar.prototype.clean"></a>[function <span class="apidocSignatureSpan">inquirer.ui.BottomBar.prototype.</span>clean ()](#apidoc.element.inquirer.ui.BottomBar.prototype.clean)
- description and source-code
```javascript
clean = function () {
  rlUtils.clearLine(this.rl, this.bottomBar.split('\n').length);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.ui.BottomBar.prototype.enforceLF"></a>[function <span class="apidocSignatureSpan">inquirer.ui.BottomBar.prototype.</span>enforceLF (str)](#apidoc.element.inquirer.ui.BottomBar.prototype.enforceLF)
- description and source-code
```javascript
enforceLF = function (str) {
  return str.match(/[\r\n]$/) ? str : str + '\n';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.ui.BottomBar.prototype.render"></a>[function <span class="apidocSignatureSpan">inquirer.ui.BottomBar.prototype.</span>render ()](#apidoc.element.inquirer.ui.BottomBar.prototype.render)
- description and source-code
```javascript
render = function () {
  this.write(this.bottomBar);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.ui.BottomBar.prototype.updateBottomBar"></a>[function <span class="apidocSignatureSpan">inquirer.ui.BottomBar.prototype.</span>updateBottomBar (bottomBar)](#apidoc.element.inquirer.ui.BottomBar.prototype.updateBottomBar)
- description and source-code
```javascript
updateBottomBar = function (bottomBar) {
  this.bottomBar = bottomBar;
  rlUtils.clearLine(this.rl, 1);
  this.rl.output.unmute();
  this.clean().render();
  this.rl.output.mute();
  return this;
}
```
- example usage
```shell
...

// Or simply write output
ui.log.write('something just happened.');
ui.log.write('Almost over, standby!');

// During processing, update the bottom bar content to display a loader
// or output a progress bar, etc
ui.updateBottomBar('new bottom bar content');
'''

<a name="reactive"></a>
## Reactive interface


Internally, Inquirer uses the [JS reactive extension](https://github.com/Reactive-Extensions/RxJS) to handle events and async flows
.
...
```

#### <a name="apidoc.element.inquirer.ui.BottomBar.prototype.write"></a>[function <span class="apidocSignatureSpan">inquirer.ui.BottomBar.prototype.</span>write (message)](#apidoc.element.inquirer.ui.BottomBar.prototype.write)
- description and source-code
```javascript
write = function (message) {
  var msgLines = message.split(/\n/);
  this.height = msgLines.length;

  // Write message to screen and setPrompt to control backspace
  this.rl.setPrompt(_.last(msgLines));

  if (this.rl.output.rows === 0 && this.rl.output.columns === 0) {
<span class="apidocCodeCommentSpan">    /* When it's a tty through serial port there's no terminal info and the render will malfunction,
       so we need enforce the cursor to locate to the leftmost position for rendering. */
</span>    rlUtils.left(this.rl, message.length + this.rl.line.length);
  }
  this.rl.output.write(message);
}
```
- example usage
```shell
...
'''javascript
var ui = new inquirer.ui.BottomBar();

// pipe a Stream to the log zone
outputStream.pipe(ui.log);

// Or simply write output
ui.log.write('something just happened.');
ui.log.write('Almost over, standby!');

// During processing, update the bottom bar content to display a loader
// or output a progress bar, etc
ui.updateBottomBar('new bottom bar content');
'''
...
```

#### <a name="apidoc.element.inquirer.ui.BottomBar.prototype.writeLog"></a>[function <span class="apidocSignatureSpan">inquirer.ui.BottomBar.prototype.</span>writeLog (data)](#apidoc.element.inquirer.ui.BottomBar.prototype.writeLog)
- description and source-code
```javascript
writeLog = function (data) {
  this.rl.output.unmute();
  this.clean();
  this.rl.output.write(this.enforceLF(data.toString()));
  this.render();
  this.rl.output.mute();
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.inquirer.ui.BottomBar.super_.prototype"></a>[module inquirer.ui.BottomBar.super_.prototype](#apidoc.module.inquirer.ui.BottomBar.super_.prototype)

#### <a name="apidoc.element.inquirer.ui.BottomBar.super_.prototype.close"></a>[function <span class="apidocSignatureSpan">inquirer.ui.BottomBar.super_.prototype.</span>close ()](#apidoc.element.inquirer.ui.BottomBar.super_.prototype.close)
- description and source-code
```javascript
close = function () {
  // Remove events listeners
  this.rl.removeListener('SIGINT', this.onForceClose);
  process.removeListener('exit', this.onForceClose);

  this.rl.output.unmute();

  if (this.activePrompt && typeof this.activePrompt.close === 'function') {
    this.activePrompt.close();
  }

  // Close the readline
  this.rl.output.end();
  this.rl.pause();
  this.rl.close();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.ui.BottomBar.super_.prototype.onForceClose"></a>[function <span class="apidocSignatureSpan">inquirer.ui.BottomBar.super_.prototype.</span>onForceClose ()](#apidoc.element.inquirer.ui.BottomBar.super_.prototype.onForceClose)
- description and source-code
```javascript
onForceClose = function () {
  this.close();
  console.log('');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.inquirer.ui.Prompt"></a>[module inquirer.ui.Prompt](#apidoc.module.inquirer.ui.Prompt)

#### <a name="apidoc.element.inquirer.ui.Prompt.Prompt"></a>[function <span class="apidocSignatureSpan">inquirer.ui.</span>Prompt (prompts, opt)](#apidoc.element.inquirer.ui.Prompt.Prompt)
- description and source-code
```javascript
Prompt = function (prompts, opt) {
  Base.call(this, opt);
  this.prompts = prompts;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.ui.Prompt.super_"></a>[function <span class="apidocSignatureSpan">inquirer.ui.Prompt.</span>super_ (opt)](#apidoc.element.inquirer.ui.Prompt.super_)
- description and source-code
```javascript
super_ = function (opt) {
  // Instantiate the Readline interface
  // @Note: Don't reassign if already present (allow test to override the Stream)
  if (!this.rl) {
    this.rl = readline.createInterface(setupReadlineOptions(opt));
  }
  this.rl.resume();

  this.onForceClose = this.onForceClose.bind(this);

  // Make sure new prompt start on a newline when closing
  this.rl.on('SIGINT', this.onForceClose);
  process.on('exit', this.onForceClose);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.inquirer.ui.Prompt.prototype"></a>[module inquirer.ui.Prompt.prototype](#apidoc.module.inquirer.ui.Prompt.prototype)

#### <a name="apidoc.element.inquirer.ui.Prompt.prototype.fetchAnswer"></a>[function <span class="apidocSignatureSpan">inquirer.ui.Prompt.prototype.</span>fetchAnswer (question)](#apidoc.element.inquirer.ui.Prompt.prototype.fetchAnswer)
- description and source-code
```javascript
fetchAnswer = function (question) {
  var Prompt = this.prompts[question.type];
  this.activePrompt = new Prompt(question, this.rl, this.answers);
  return rx.Observable.defer(function () {
    return rx.Observable.fromPromise(this.activePrompt.run().then(function (answer) {
      return {name: question.name, answer: answer};
    }));
  }.bind(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.ui.Prompt.prototype.filterIfRunnable"></a>[function <span class="apidocSignatureSpan">inquirer.ui.Prompt.prototype.</span>filterIfRunnable (question)](#apidoc.element.inquirer.ui.Prompt.prototype.filterIfRunnable)
- description and source-code
```javascript
filterIfRunnable = function (question) {
  if (question.when === false) {
    return rx.Observable.empty();
  }

  if (!_.isFunction(question.when)) {
    return rx.Observable.return(question);
  }

  var answers = this.answers;
  return rx.Observable.defer(function () {
    return rx.Observable.fromPromise(
      runAsync(question.when)(answers).then(function (shouldRun) {
        if (shouldRun) {
          return question;
        }
      })
    ).filter(function (val) {
      return val != null;
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.ui.Prompt.prototype.onCompletion"></a>[function <span class="apidocSignatureSpan">inquirer.ui.Prompt.prototype.</span>onCompletion (answers)](#apidoc.element.inquirer.ui.Prompt.prototype.onCompletion)
- description and source-code
```javascript
onCompletion = function (answers) {
  this.close();

  return answers;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.ui.Prompt.prototype.processQuestion"></a>[function <span class="apidocSignatureSpan">inquirer.ui.Prompt.prototype.</span>processQuestion (question)](#apidoc.element.inquirer.ui.Prompt.prototype.processQuestion)
- description and source-code
```javascript
processQuestion = function (question) {
  question = _.clone(question);
  return rx.Observable.defer(function () {
    var obs = rx.Observable.of(question);

    return obs
      .concatMap(this.setDefaultType.bind(this))
      .concatMap(this.filterIfRunnable.bind(this))
      .concatMap(utils.fetchAsyncQuestionProperty.bind(null, question, 'message', this.answers))
      .concatMap(utils.fetchAsyncQuestionProperty.bind(null, question, 'default', this.answers))
      .concatMap(utils.fetchAsyncQuestionProperty.bind(null, question, 'choices', this.answers))
      .concatMap(this.fetchAnswer.bind(this));
  }.bind(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.ui.Prompt.prototype.run"></a>[function <span class="apidocSignatureSpan">inquirer.ui.Prompt.prototype.</span>run (questions)](#apidoc.element.inquirer.ui.Prompt.prototype.run)
- description and source-code
```javascript
run = function (questions) {
  // Keep global reference to the answers
  this.answers = {};

  // Make sure questions is an array.
  if (_.isPlainObject(questions)) {
    questions = [questions];
  }

  // Create an observable, unless we received one as parameter.
  // Note: As this is a public interface, we cannot do an instanceof check as we won't
  // be using the exact same object in memory.
  var obs = _.isArray(questions) ? rx.Observable.from(questions) : questions;

  this.process = obs
    .concatMap(this.processQuestion.bind(this))
    // 'publish' creates a hot Observable. It prevents duplicating prompts.
    .publish();

  this.process.connect();

  return this.process
    .reduce(function (answers, answer) {
      _.set(this.answers, answer.name, answer.answer);
      return this.answers;
    }.bind(this), {})
    .toPromise(Promise)
    .then(this.onCompletion.bind(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.inquirer.ui.Prompt.prototype.setDefaultType"></a>[function <span class="apidocSignatureSpan">inquirer.ui.Prompt.prototype.</span>setDefaultType (question)](#apidoc.element.inquirer.ui.Prompt.prototype.setDefaultType)
- description and source-code
```javascript
setDefaultType = function (question) {
  // Default type to input
  if (!this.prompts[question.type]) {
    question.type = 'input';
  }
  return rx.Observable.defer(function () {
    return rx.Observable.return(question);
  });
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
