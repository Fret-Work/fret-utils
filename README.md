# FRET-Utils
#### Matt Luckcuck and Marie Farrell

## fretish.sty

A LaTeX Style File for writing/writing about `FRETish`.

### Usage

* Add `\usepackage{fretish}` to the preable of your LaTeX source file.
* To print the components of a `FRETish` requirement, you can use `fretishComponents{}` (or `\fretishComponentsSmall{}` if the other command is too wide, this seems to work well in IEEE two-column).
* Each field (component) of a `FRETish` requirement has two commands:
    - A command starting with an uppercase letter prints the name of that part in the right `Fretish` colour, e.g. `\Condition{}` prints "Condition" in orange.
    - A command starting with a lowercase letter takes 1 argument and prints that argument in the right `Fretish` colour for that part of the requirement, e.g. `\condition{if x >= 5 }` prints "if x >= 5" in orange. 
* The `\frettext` command lets you typeset a full string of `FRETish` text, it has one parameter for each field and if you have nothing for a particular field just use empty braces ("`{}`")