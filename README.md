# RethinkDB fork of Quickjspp

This is forked from https://github.com/c-smile/quickjspp , a fork of
Fabrice Bellard's QuickJS that adds Windows support and other extras.

The purpose of this branch is for inclusion into RethinkDB as its
JavaScript engine, so that RethinkDB's Windows release can include the
`r.js` command.

It makes the following changes, relative to quickjspp:

- This omits some of the c-smile commits relating to JSX and storage.
  The purpose of this is to reduce the size of the changeset relative
  to Bellard's QuickJS.

- This applies some of Bellard's latest changes, at
  https://github.com/bellard/quickjs , that were made after the most
  recent release, 2021-03-27.  (This includes a bugfix commit.)

- It has some other minor changes.

The quickjspp README continues below...



# QuickJS Javascript Engine 

Authors: Fabrice Bellard and Charlie Gordon

Ported from https://bellard.org/quickjs/ and its official GitHub mirror https://github.com/bellard/quickjs

By Andrew Fedoniouk (a.k.a. c-smile)

This version is 

* Microsoft Visual C++ compatible/compileable
* Is used in Sciter.JS
* It contains extras, check [wiki](https://github.com/c-smile/quickjspp/wiki) 

The main documentation is in doc/quickjs.pdf or doc/quickjs.html.

# Build using Microsoft Visual Studio (2017 or 2019)

Prerequisite: **premake5** - [download](https://premake.github.io/download.html) and install it.

Then go to /win folder and run premake-vs2017.bat or premake-vs2019.bat . 

It will generate .build/vs2017/quickjs-msvc.sln and open it in Microsoft Visual Studio.

Press F5 to compile it and run qjs - interactive JS command line application.




