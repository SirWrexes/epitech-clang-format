# **EPITECH CLang-Format config**
# Because Norminettes are broken as hell.
***

## Several reasons why:
1. #### Norminettes are __all broken__.
    * Not kept up to date
    * Flag tons of false positives
    * They use and old version of Epitech's coding style  and it's _hard-coded_ inside them
    -- really this sucks and disallows any kind of flexibility.
    And if you know me, you know I LOVE flexible code


2. #### Norminettes are __forbidden__... unless you make one yourself.
    * Making a C parser is lot of work and often not worth it :
    It'll teach you very interresting things but I'm ready to bet that if you're
    not a geius that has 100% for every project ─ and if you are you don't
    need a norminette ─ your parser will end up exactly like NormEZ : broken as hell.


3. #### CLang and its tools are awesome !

    * You should really take time to check them out, it's worth your while.
    * CLang is an amazing compiler :
        * Faster than GCC
        * Much more eligible error/warning messages
        * GCC compatible: Compile options and GNU C extensions still work great with it !


4. #### I'll probably have typed more text in this README than in my config
    * Which proves how easy it is to have a functional way of making both your C and C++
    code Epitech Style compliant, while being able to
    [integrate it with your favorite editor/IDE](https://clang.llvm.org/docs/ClangFormat.html).


5. ### Last but not least: it's just a config file
    * Super easy to update !
    * Super easy to adapt it to your needs !
***

## Installation:
Go in your home directory and execute the following commands
```bash
$ git clone git@github.com:fox-tek/.clang-format.git
$ ln -s .clang-format/.clang-format .
```
__Note:__ Of course, you can chose to download the repo to some other directory like, say, `$HOME/.config/`
***

## Command line usage:
I invite you to type the following command in a terminal and carefuly read its output.
```bash
$ clang-format -help
```
***

## Integration with your editor:
* __Vim, Emacs, Clion, VSCode, BBEdit:__ go [here](https://clang.llvm.org/docs/ClangFormat.html)
* __Sublime Text:__ Check [this](https://packagecontrol.io/packages/Clang%20Format) out. _(You're welcome, Raphael)_
* __Notepad++:__ Bruh.
***

## List of rules implemented
* __L - Layout inside a function scope__
    * ⬇ L2 - Indentation
#### CLang can't handle these :
And some of them a Norminette can't handle either.
_You should know the style requiremments anyway._
* __O - File organization__
    * ⬆ O1 - Contents of the delivery folder
    * O2 - File extension
    * O3 - File coherence
    * O4 - Naming files and folders
* __G - Global scope__
    * G1 - File header
* __F - Functions__
    * F1 - Coherence of functions
    * F2 -  Naming functions
* __V - Variables and types__
    * V1 - Naming identifiers
    * V2 - Structures
* __I'll finish this later.__
    * and start actually writing the config file.
