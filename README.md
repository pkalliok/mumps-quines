# MUMPS quines

These are [quines](https://en.wikipedia.org/wiki/Quine_%28computing%29)
in the programming language [MUMPS](https://en.wikipedia.org/wiki/MUMPS). 

Just to show that you can.

- [Quine 1](./quine1.mps) cheats by using the introspective $t function
  to read its own code.

- [Quine 2](./quine2.mps) leverages the fact that you can dynamically
  execute code from strings with the X command.  Then the program can
  read itself from the same string it is being executed from.

- [Quine 3](./quine3.mps) is a "traditional" quine in that it doesn't
  use any language-specific quirks.  It just reconstructs itself from a
  string containing its textual representation.

