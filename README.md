pyle is a lexer for Python that I wrote from scratch. You can run it with:

    cabal configure
    cabal build
    ./dist/build/pick-lex/pick-lex < $STUFF

You can test the lexer on real python files, or you can pump the files in
`tests/test_lexer/`. The files with the suffix `.txt` are the raw files, while
the files with the suffix `.txt.res` are the target results.

pyle is pretty bare-bones. We do not currently support:

  * unicode (I know, I know)
  * bytestrings
  * unicode bytestrings!
  * tabs, because they're evil. (just kidding; it's because I'm lazy)

... but it is enough to do some interesting things.

pyle is distributed with an MIT license which basically lets you use it for
almost anything, as long as you keep the license in the project, and don't
take my name off of the stuff I wrote.