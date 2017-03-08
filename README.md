Sources copied/slightly modified from : [https://github.com/software-engineering-amsterdam/myriad-ql/tree/elmos-dev/elmos]

Steps to reproduce:

1. Clone project
2. Open atom in root dir
3. Open src/UI/QLSFormRenderer
4. Go to line 76
5. Put your cursor right behind SingleChildSection and press space




**Atom**: 1.14.4 ia32
**Electron**: 1.3.13
**OS**: Microsoft Windows 7 Professional 
**Thrown From**: [elmjutsu](https://github.com/halohalospecial/atom-elmjutsu) package 5.2.0


### Stack Trace

Uncaught RangeError: Maximum call stack size exceeded

```
At C:\Users\Paco\.atom\packages\elmjutsu\elm\indexer.js:1278

RangeError: Maximum call stack size exceeded
    at Function.func (/packages/elmjutsu/elm/indexer.js:1278:11)
    at A2 (/packages/elmjutsu/elm/indexer.js:92:11)
    at /packages/elmjutsu/elm/indexer.js:1004:9)
    at A3 (/packages/elmjutsu/elm/indexer.js:98:11)
    at Function.func (/packages/elmjutsu/elm/indexer.js:1272:10)
    at A2 (/packages/elmjutsu/elm/indexer.js:92:11)
    at /packages/elmjutsu/elm/indexer.js:10297:18
    at /packages/elmjutsu/elm/indexer.js:16:54
    at Function.func (/packages/elmjutsu/elm/indexer.js:1278:11)
    at A2 (/packages/elmjutsu/elm/indexer.js:92:11)
    at /packages/elmjutsu/elm/indexer.js:1004:9)
    at A3 (/packages/elmjutsu/elm/indexer.js:98:11)
    at Function.func (/packages/elmjutsu/elm/indexer.js:1272:10)
    at A2 (/packages/elmjutsu/elm/indexer.js:92:11)
    at /packages/elmjutsu/elm/indexer.js:10297:18
    at /packages/elmjutsu/elm/indexer.js:16:54
    at Function.func (/packages/elmjutsu/elm/indexer.js:1278:11)
    at A2 (/packages/elmjutsu/elm/indexer.js:92:11)
    at /packages/elmjutsu/elm/indexer.js:1004:9)
    at A3 (/packages/elmjutsu/elm/indexer.js:98:11)
    at Function.func (/packages/elmjutsu/elm/indexer.js:1272:10)
    at A2 (/packages/elmjutsu/elm/indexer.js:92:11)
    at /packages/elmjutsu/elm/indexer.js:10297:18
    at /packages/elmjutsu/elm/indexer.js:16:54
    at Function.func (/packages/elmjutsu/elm/indexer.js:1278:11)
    at A2 (/packages/elmjutsu/elm/indexer.js:92:11)
    at /packages/elmjutsu/elm/indexer.js:1004:9)
    at A3 (/packages/elmjutsu/elm/indexer.js:98:11)
    at Function.func (/packages/elmjutsu/elm/indexer.js:1272:10)
    at A2 (/packages/elmjutsu/elm/indexer.js:92:11)
```

### Commands

```
     -5:28.3.0 core:backspace (input.hidden-input)
```

### Non-Core Packages

```
elm-format 2.1.0 
elmjutsu 5.2.0 
language-elm 1.5.0 
linter 1.11.23 
linter-elm-make 0.22.5 
tab-switcher 1.5.4 
```

