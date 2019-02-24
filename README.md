# A Perl::Tidy `.perltidyrc` with a Prettier style

[Perl Style](https://perldoc.perl.org/perlstyle.html) and later [Perl Best Practices](http://shop.oreilly.com/product/9780596001735.do) defined a Perl style. But _Tim Toady_...

[Perltidy](https://github.com/perltidy/perltidy) ([website](https://perltidy.github.io/perltidy/) and [older website](http://perltidy.sourceforge.net/)), sometimes called Perl::Tidy or PerlTidy, is a formatter for Perl. It has a lot of options.

[Prettier](https://github.com/prettier/prettier) ([website](https://prettier.io/)) is an opinionated code formatter for JavaScript and other web languages (TypeScript, JSON, HTML, CSS, etc.). Opinionated means that it has few options.

This is a simple configuration file for Perltidy (a `.perltidyrc` runcom file) that tries to mimic the default Prettier style.

## Rationale

Everyone hates what a code formatter does to their code. And everyone loves what a code formatter does to other people code.

But the great formatting war is not about spaces _vs_ tabs (spaces!), nor if semi-colons should be used (duh!), not even between opening braces on the same or on a new line (same!). The war is between freedom (TIMTOWTDI!) and just one style: experiments like `gofmt` and Prettier [try](https://prettier.io/docs/en/why-prettier.html) to solve this eternal debate, removing it from programmers and leaving them with more free time for important stuff.

So please, use a formatter and don't argue with your cow-workers. And if you write modern Perl code for the web and you want it to blend into the common style, try this style.

## Rules

Prettier is generally more compact than Perltidy default.

- 80 chars lines (configurable in Prettier)
- 2 chars "tab" (configurable in Prettier)
- keep empty lines, but collpsed into a single one
- one line if it fits, else multiline
- quotes
- semicolons (configurable in Prettier)
- bracket spacing
- `prettier-ignore`, or `prettier-ignore-start` and `prettier-ignore-end`.

In Perl we tend to add "trailing commas" (configurable, but not default, in Prettier).

## Usage

Put the `.perltidyrc` file in your home or your project directory.

Use `-b` to modify files in-place (with backup).
