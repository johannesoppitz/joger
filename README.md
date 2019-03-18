# The Joger programming language

Welcome to the Joger programming language! This is a personal project without the support of a company, organization or foundation.
Please don't expect a professional presentation yet.

Overview
--------

Joger is a high-level, general-purpose programming language inspired by the author's experience with C, D, Java and Python (and a syntax influenced by many more). Like most modern languages, Joger promises readable syntax, fast code execution, robustness and platform-independence. Have a look at the [wiki](https://github.com/johannesoppitz/joger/wiki) to get a first glance.

Installing
--------

The compiler is currently written entirely in the D programming language. You can find links to popular and free D compilers [here](https://dlang.org/download.html).
Because the project is in an early stage, it is currently built on Windows without using an IDE. Right now, you can simply execute 'make.bat' (a makefile for linux will follow soon) and play around with the debug-executable.

Joger does not compile into native binaries, but generates optimized C code. Therefore you also need to have a stable C compiler on your system, ideally with full support of C99 or later.

Testing
--------

Most functions and struct methods come with unittests. Large classes like the lexer require extensive tests which should be put in /src/compiler/test. These time- and resource-consuming tests get only executed via special program arguments
(for example, 'joger -acid_lexer' runs all the tests specified in 'acid_lexer.d').

Development Process
--------

Joger is currently being developed using strict documentation-driven design. Adding, editing and removing features always happens in four steps:
1. The wiki gets updated.
2. The unittests, testing modules and test ressources get updated.
3. The actual source code gets updated and tested until the software passes all tests.
4. The master branch on GitHub gets updated.

Copyright and License Information
--------

Joger is distributed under the terms of the MIT license. See [LICENSE](https://github.com/johannesoppitz/joger/blob/master/LICENSE) for details.
