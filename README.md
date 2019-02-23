# perltidy-prettier-style
Perltidy runcom file for a Prettier style

[Perl Style](https://perldoc.perl.org/perlstyle.html) and later [Perl Best Practices](http://shop.oreilly.com/product/9780596001735.do) defined Perl style.
[Perltidy](https://github.com/perltidy/perltidy) ([website](https://perltidy.github.io/perltidy/) and [older website](http://perltidy.sourceforge.net/)), sometimes called Perl::Tidy or PerlTidy, is a formatter for Perl. It has a lot of options.

[Prettier](https://github.com/prettier/prettier) ([website](https://prettier.io/)) is an opinionared code formatter for JavaScript and other web languages (HTML, CSS, etc.). Opinionated means that it has few options.

This is a simple configuration file for `perltidy` (`.perltidyrc`) that tries to mimic default Prettier style.


## Rationale

Everyone hates what a code formatter does to their code. And everyone loves what a code formatter does to other people code.

TMTOWTDI (?)

`gofmt` and `elm-format`.

If you write modern Perl code for the web and you want it to blend into the common style.


## Rules

Prettier is generally more compact than Perltidy default.

- 80 chars lines (configurable)
- 2 chars "tab" (configurable)
- keep empty lines, but collpsed into a single one
- one line if it fit, else multiline
- quotes
- semicolons (configurable)
- bracket spacing

`prettier-ignore` or `prettier-ignore-start` and `prettier-ignore-end`.

In Perl we tend to add "trailing commas" (configurable in Prettier).


## Usage

Use `-b` to modify files in-place (with backup).

