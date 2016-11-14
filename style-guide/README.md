#Style

A guide for programming in style

Detailed, language/framework specific style guides:

* Android
* C/C++
* C#
* Cinder
* [Git](./Git)
* [HTML](./html)
* [Javascript](./javascript)
* [Laravel](./laravel)
* Objective-C
* OpenFrameworks
* [PHP](./php)
* [Stylus](./stylus)
* Swift
* Unity
* [Vue](./vue)

## Formatting

* Avoid inline comments.
* Break long lines after 100 characters.
* Delete trailing whitespace.
* Don't` misspell.
* Use an empty line between methods.
* Use spaces around operators, except for unary operators, such as `!`. 
* Use spaces after commas, after colons and semicolons, around `{` and before `}`.


## Naming

* Avoid abbreviations.
* Avoid object types in names (`user_array`, `email_method`, `CalculatorClass`, `ReportModule`) use instead (`users`, `send_email`, `Calculator`, `Reports`).
* Name variables, methods, and classes to reveal intent.
* Treat acronyms as words in names such as (`XmlHttpRequest` not `XMLHTTPRequest`).
 
 
## Organization
 
* Order methods so that caller methods are earlier in file than the methods they call.
* Order methods so that methods are as close as possible to other methods they call.