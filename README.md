# Funkin' Code CookBook
## [**READ THE DOCUMENTATION HERE**](https://thekade.net/funkin-cookbook/)

Forked from [Haxe Code CookBook](https://github.com/HaxeFoundation/code-cookbook), this is a one stop shop for all Funkin' Modding Tutorials!

## Running a local copy

You need [Haxe 3.4.2+](https://haxe.org/download/list/) installed.

The static site generator source depends on [hxtemplo](https://lib.haxe.org/p/hxtemplo) and [haxe-markdown](https://lib.haxe.org/p/markdown).

Install the libraries using haxelib, run the following command in the root of the project:
```
haxelib install all
```
The CSS files are compressed using [less](http://lesscss.org/#using-less). 
Install from npm:
```
npm install
```

Either run `build.bat` or `build.sh` depending on your platform.

(joke is, they're the same file)

The main repo tells users to run it through neko, so we do that as well. But we also run highlighting.hxml for the code highlighting.

For highlighting you'll need the submodules in `grammars/` (XML and JSON have some git errors, so just manually download them.)