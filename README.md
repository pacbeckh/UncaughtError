Sources copied/slightly modified from : [https://github.com/software-engineering-amsterdam/myriad-ql/tree/elmos-dev/elmos]

Steps to reproduce:

1. Clone project https://github.com/pacbeckh/UncaughtError
2. Open atom in root directory
3. Open file `tests\QL\TypeChecker\Expressions\OperandTypesTests.elm`
4. Remove the above file in Atom 

Demo:
![ScreenCapture](https://github.com/pacbeckh/UncaughtRangeError/blob/master/UncaughtError.gif)

**Atom**: 1.15.0 ia32
**Electron**: 1.3.13
**OS**: Microsoft Windows 7 Professional 
**Thrown From**: [elmjutsu](https://github.com/halohalospecial/atom-elmjutsu) package 5.3.3



### Stack Trace

Uncaught Error: ENOENT: no such file or directory, open 'C:\Users\Paco\Elm\UncaughtRangeError\tests\QL\TypeChecker\Expressions\OperandTypesTests.elm'

```
At fs.js:640

Error: ENOENT: no such file or directory, open 'C:\Users\Paco\Elm\UncaughtRangeError\tests\QL\TypeChecker\Expressions\OperandTypesTests.elm'
    at Error (native)
    at Object.fs.openSync (fs.js:640:18)
    at Object.module.(anonymous function) [as openSync] (ELECTRON_ASAR.js:168:20)
    at Object.fs.readFileSync (fs.js:508:33)
    at Object.fs.readFileSync (ELECTRON_ASAR.js:501:29)
    at Object.sendFileContentsChanged (/packages/elmjutsu/lib/indexing.js:16:21)
    at /packages/elmjutsu/lib/core.js:117:20
    at Function.module.exports.Emitter.simpleDispatch (/app.asar/node_modules/event-kit/lib/emitter.js:25:14)
    at Emitter.module.exports.Emitter.emit (/app.asar/node_modules/event-kit/lib/emitter.js:129:28)
    at TextEditor.module.exports.TextEditor.destroyed (/app.asar/src/text-editor.js:574:20)
    at TextEditor.module.exports.Model.destroy (/app.asar/src/model.js:31:58)
    at /app.asar/node_modules/tree-view/lib/tree-view.js:1034:30)
    at ApplicationDelegate.module.exports.ApplicationDelegate.confirm (/app.asar/src/application-delegate.js:206:49)
    at AtomEnvironment.module.exports.AtomEnvironment.confirm (/app.asar/src/atom-environment.js:934:39)
    at TreeView.module.exports.TreeView.removeSelectedEntries (/app.asar/node_modules/tree-view/lib/tree-view.js:1019:19)
    at /app.asar/node_modules/tree-view/lib/main.js:67:39)
    at CommandRegistry.module.exports.CommandRegistry.handleCommandEvent (/app.asar/src/command-registry.js:259:29)
    at /app.asar/src/command-registry.js:3:59
    at KeymapManager.module.exports.KeymapManager.dispatchCommandEvent (/app.asar/node_modules/atom-keymap/lib/keymap-manager.js:599:16)
    at KeymapManager.module.exports.KeymapManager.handleKeyboardEvent (/app.asar/node_modules/atom-keymap/lib/keymap-manager.js:390:22)
    at WindowEventHandler.module.exports.WindowEventHandler.handleDocumentKeyEvent (/app.asar/src/window-event-handler.js:106:36)
    at /app.asar/src/window-event-handler.js:3:59)
```

### Commands

```
     -0:14.9.0 tree-view:remove (ol.tree-view.full-menu.list-tree.has-collapsable-children.focusable-panel)
```

### Non-Core Packages

```
busy-signal 1.3.0 
elm-format 2.1.0 
elmjutsu 5.3.3 
intentions 1.1.2 
language-elm 1.5.0 
linter 2.1.0 
linter-elm-make 0.23.0 
linter-ui-default 1.1.0 
tab-switcher 1.5.4 
```


Also reproduced by @stil4m on OSX 10.12
