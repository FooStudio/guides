# Stylus

* Styles are component scoped, and should be at most cases.
* Use [Sanitize.css](https://jonathantneal.github.io/sanitize.css/) for browser rendering consistency.
* Use [Rupture](http://jescalan.github.io/rupture/) as media query utility.
* Use [LostGrid](http://lostgrid.org/) as grid system.
* Use [PostStylus](https://github.com/seaneking/poststylus) to load [PostCSS](https://github.com/postcss/postcss) plugins.
* Use [Nib](https://github.com/tj/nib) for mixins, utilities, etc.
* Use [Rucksack](http://simplaio.github.io/rucksack/docs/) for more utilities and mixins.
* Avoid, when possible, having files longer than 100 lines.

## Formatting

* Prefer omitting braces.
* Prefer omitting semicolons.
* Use `$` when naming variables (`$red = #ff0000`).
* Avoid using shorthand properties for only one value: `background-color #ff0000`, not `background #ff0000`.
* Use double quotation marks.
* Use only lowercase, except for hex, string values of component classes.
* Don't add a unit specification after `0` values, unless required by a mixin.
* Use double colons for pseudo-elements.

## Order

* Place `@extends` at the top of your declaration list.
* Place media queries directly after the declaration list.
* Place concatenated selectors second.
* Place pseudo-elements and pseudo-states third.
* Place nested elements fourth.
* Place nested classes fifth.

## Selectors

* **Avoid nesting more than 2 selectors deep.**
* Don't use ID's for styling.
* Use meaningful names: `$visual-grid-color` not `$color` or `$vslgrd-clr`.
* Use ID and class names that are as short as possible but as long as necessary. 
* Avoid using the direct descendant operator `>`. 
* Avoid nesting within a media query.
