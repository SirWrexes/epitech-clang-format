# **EPITECH CLang-Format config**
# Because Norminettes are broken as hell.
***

## Several reasons why:
1. #### Norminettes are __all broken__.
    * Mostly not kept up to date
    * Usually flag tons of false positives
    * They use and old version of Epitech's coding style and it's _hard-coded_ inside them
    -- really this sucks and disallows any kind of flexibility.
    And if you know me, you know I LOVE flexible code


2. #### Norminettes are __forbidden__... unless you make one yourself.
    * Making a C parser is a lot of work and often not worth it :
    It'll teach you very interresting things but I'm ready to bet that if you're
    not a genius that has 100% to every project ─ and in that case you wouldn't need
    a norminette ─ your parser will end up exactly like NormEZ : broken as hell.


3. #### CLang and its tools are awesome !
    * You should really take time to check them out, it's worth your while.
    * `clang-format` reformats your code directly, and either prints it to stdout or directly in place, you chose.
    * CLang is an amazing compiler :
        * Faster than GCC
        * Much more eligible error/warning messages
        * GCC compatible: Compile options and GNU C extensions still work great with it !


4. #### I'll probably have typed more text in this README than in my config
    * Which proves how easy it is to have a functional way of making both your C and C++
    code Epitech Style compliant, while being able to
    [integrate it with your favorite editor/IDE](https://clang.llvm.org/docs/ClangFormat.html).


5. #### Last but not least: it's just a config file
    * Super easy to update !
    * Super easy to adapt it to your needs !
***

## Installation:
Go in your home directory and execute the following commands
```bash
$ git clone git@github.com:fox-tek/epitech-clang-format.git
$ ln -sf epitech-clang-format/.clang-format ~/
```
__Note:__ Of course, you can chose to download the repo to some other directory like, say, `$HOME/.config/`
***

## Command line usage:
Run the following command in a terminal and carefuly read its output.
```bash
$ clang-format --help
```
***

## Integration with your editor:
* __Vim, Emacs, VSCode, BBEdit:__ go [here](https://clang.llvm.org/docs/ClangFormat.html)
* __CLion__: Read [CLion documentation](https://www.jetbrains.com/help/clion/clangformat-as-alternative-formatter.html)
* __Sublime Text:__ Check [this](https://packagecontrol.io/packages/Clang%20Format) out.
* __Nano:__ Bruh.
***

## What rules are implemented ?
Open the .clang-format and read. I made it so it's clear what it does. Happy coding ! 😉
***

## Known issues:
* #### Rules that take "Never" as value trigger an error
Update Clang-Format to the latest version. This has been made for clang-format 9.0.1, I can't assure you it'll work on previous iterations.
* #### Instructionless while/for
`while(SOME_CONDITION); ` will be converted to ` while(SOME_CONDITION)\n;` (where `\n` is an actual linebreak). Just do `while(SOME_CONDITION) {}`.
