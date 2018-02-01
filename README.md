# MarkSimple

[![Build Status](https://travis-ci.org/bueltge/marksimple.svg?branch=master)](https://travis-ci.org/bueltge/marksimple)
[![Maintainability](https://api.codeclimate.com/v1/badges/3ce79c7b4118c47951cc/maintainability)](https://codeclimate.com/github/bueltge/marksimple/maintainability)

A simple Markdown parser, short and only with the rules there I currently need. The function is regex based and it is possible to enhance your custom rules.

---

Yes, **I know**, it give a lot of __open projects__ that solve the same goal. However it was fun to write my custom parser, only with the rules there I need, not to much overhead. Yes, also I mean that other packages more solid solid, lof of usages, bot not points enough to learn about regex and markdown. Besides *I know* a regex parser is not the best, fastest way, but also here, _I would to teach me in this context_.

## Demo, Tests
The solution is still active in his tests, you find it [here](https://bueltge.de/MarkSimple/test/). This test of the class is also build as [PWA](https://developers.google.com/web/progressive-web-apps/), Progressive Web App. It was only an fun project for me to understand it on a really simple site how it works. But is important, if you see the directory `test` in this repository here and wounder about so much files there are not in the context of the Markdown parser. If you will check the PWA, use it on your mobile or play with Chrome/WebInspector.

## Active use
The class is simple and I use it for my own documentation, there I write in markdown. Here and there is the result a single oage to help in each day to find the right syntax, hints, background and others. You can see this on this examples:

 * [MarkSimple Tests](https://bueltge.de/MarkSimple/test/)
 * [My Git Notes](https://bueltge.de/git/)
 * [My Markdown Notes](https://bueltge.de/md/)
 * [My Linux command notes](https://bueltge.de/linux/)

## Support
My class supports currently the follow syntax. But Pull Request are really welcome and the solution give you the possibility to add your own rule.

 * Headers, `h1` - `h6` - `#` to `######` before the string
 * Image, `![](path/to/image.png "Alt text")`
 * Strong, bold text, `strong` - `**` or `__` before and after the string
 * Italic text, `em` - an `*` or `_` before and after the string
 * Unordered list, `ul` - `*` for each line
 * Inline Code, `code` - an ``` backtick before and after the code string
 * Code Blocks, `pre` - `    ` (4 spaces) or `	` (tab) in each line or the fenced code blocks by placing triple backticks and optional the language identifier,
 * Links, `a` - `[Link Text](Link URL)`
 * Horizontal line, `---`
 * Break, new line, `<br>`

## Usage
#### Requirements
 * PHP 7

Install static via download, clone the repository or use dependency management via Composer `composer require bueltge/marksimple`

You find the solution and the tests in the [repository on GitHub](https://github.com/bueltge/marksimple).

See the test directory for an example with two different usages. The test directory works as PWA, for examples see only the file `index.php`.

#### Code examples
    // Example with four spaces.
    require_once '../vendor/autoload.php';
    use Bueltge\Marksimple\Marksimple as MS;
    print (new MS('../README.md'));

```php
// Example Github Code Block ```php.
require_once '../vendor/autoload.php';
use Bueltge\Marksimple\Marksimple as MS;
print (new MS('../README.md'));
```

## Kudos
On the way to the goal of my simple parser I use lot of tests, tries on the online Regex testers. Thanks a lot to the authors of this followed two sites, great!

 * [regular expressions 101](https://regex101.com/)
 * [DebuggexBeta](https://www.debuggex.com/)
 * [Learn Regex The Easy Way](https://github.com/zeeshanu/learn-regex)

## License
Copyright (c) 2017 [Frank Bültge](https://bueltge.de)

Good news, this plugin is free for everyone! Since it's released under the [MIT License](https://github.com/inpsyde/marksimple/blob/master/LICENSE) you can use it free of charge on your personal or commercial website.

## Contributing
 * [GitHub Repository](https://github.com/bueltge/marksimple)

All feedback / bug reports / pull requests are welcome.

---
