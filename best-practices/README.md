# Best Practices

A guide for programming well.

## General

* These are not to be blindly followed; strive to understand these and ask when in doubt.
* Don't duplicate the functionality of a built-in library.
* Don't swallow exceptions o "fail silently".
* Keep code simple.

## Object-Oriented Design

* Avoid global variables.
* Avoid long parameter lists.
* Prefer composition over inheritance.
* Prefer small methods. Between 1 and 10 lines is best.
* Prefer small classes with a single, well-defined responsibility. When a class exceeds 100 lines, it may be doping to many things.
* [Tell, don't ask](https://robots.thoughtbot.com/tell-dont-ask)

## Email

* Use [SendGrid](https://devcenter.heroku.com/articles/sendgrid) or [Amazon SES](https://aws.amazon.com/ses/) to deliver email in staging or production environments.

## Javascript

* Use [Yarn](https://yarnpkg.com/) as dependency manager.
* Use the latest stable Javascript syntax with a transpiler, such as [babel](http://babeljs.io/).

## HTML

* Don't use a reset button on forms.
* Use `<button>` tags over `<a>` for actions.

## CSS

* Use Stylus.
* Use autoprefixer to generate vendor prefixes based on the project specific browser support that is needed.
* Prefer `overflow auto` over `overflow scroll`, because `scroll` will always display scrollbars outside of OS X, even when the content fits the container.
* Prefer mixins to `@extends`.

## Browsers

* Avoid supporting versions of Internet Explorer before IE9.

