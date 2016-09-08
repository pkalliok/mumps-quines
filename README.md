# MUMPS quines

These are [quines](https://en.wikipedia.org/wiki/Quine_%28computing%29)
in the programming language [MUMPS](https://en.wikipedia.org/wiki/MUMPS).
Just to show that you can.

Actually, you can very well.  MUMPS, while not designed especially for
quines, is from the era when self-referencing (and self-modifying) code
was a given, so it has numerous primitives that make it remarkably
easier to write quines: eval (called "XECUTE"), expression eval (called
indirection), introspective facilities for source code (called "$TEXT")
and so on.

In its own way, MUMPS is quite alike today's scripting languages, but
like most other languages of its era, has weird quirks such as
space-sensitive syntax and commands you can abbreviate.  And some
primitives like string substitution are sorely missing, as are efficient
data structures and proper function calls.

- [Quine 0](./quine0.mps) is a quine because many MUMPS implementations
  output nothing when they execute an empty source file.

- [Quine 1](./quine1.mps) cheats by using the introspective $t function
  to read its own code.

- [Quine 2](./quine2.mps) leverages the fact that you can dynamically
  execute code from strings with the X command.  Then the program can
  read itself from the same string it is being executed from.

- [Quine 3](./quine3.mps) is a "traditional" quine in that it doesn't
  use any language-specific quirks.  It just reconstructs itself from a
  string containing its textual representation.

