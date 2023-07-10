# [MathQuill](http://mathquill.com)

by [Han](http://github.com/laughinghan), [Jeanine](http://github.com/jneen), and [Mary](http://github.com/stufflebear) (<maintainers@mathquill.com>) [<img alt="slackin.mathquill.com" src="http://slackin.mathquill.com/badge.svg" align="top">](http://slackin.mathquill.com)

MathQuill is a web formula editor designed to make typing math easy and beautiful.

<h3><a href="https://niebert.github.io/mathquill/index.html" target="_blank">MathQuill GitHub Demo</a></h3>
The <a href="https://en.wikiversity.org/wiki/AppLSAC" target="_blank">MathQuill demo</a> is an  self-contained in the subdirectory `examples/` in this repository. 

* example uses `jquery-3.6.0.js` - required for MathQuill is jquery 1.5.2++
* `css/mathquill.css` generated MathQuill stylesheet  
* [Symbola fonts](https://localfonts.eu/freefonts/greek-free-fonts/unicode-fonts-for-ancient-scripts/symbola/) in `examplescss/fonts` by George Douros 

[<img alt="homepage demo" src="https://cloud.githubusercontent.com/assets/225809/15163580/1bc048c4-16be-11e6-98a6-de467d00cff1.gif" width="260">](http://mathquill.com)

The MathQuill project is supported by its [partners](http://mathquill.com/partners.html). We hold ourselves to a compassionate [Code of Conduct](http://docs.mathquill.com/en/latest/Code_of_Conduct/).

MathQuill is resuming active development and we're committed to getting things running smoothly. Find a dusty corner? [Let us know in Slack.](http://slackin.mathquill.com) (Prefer IRC? We're `#mathquill` on Freenode.)h

## Installation and Build mathquill.js 
The installation requires NodeJS to be installed on your system.

### Fetching the Open Source Code 
To fetch the source of `mathquill` call `git clone https://github.com/mathquill/mathquill.git`

### Install dependencies
As usual run `npm install` in the `mathquill` folder

### Run Make
If you run the `make` command in the `mathquill` folder, also the dependencies will be installed. 

## Getting Started

MathQuill has a simple interface. This brief example creates a MathQuill element and renders, then reads a given input:
```javascript
var htmlElement = document.getElementById('some_id');
var config = {
  handlers: { edit: function(){ ... } },
  restrictMismatchedBrackets: true
};
var mathField = MQ.MathField(htmlElement, config);

mathField.latex('2^{\\frac{3}{2}}'); // Renders the given LaTeX in the MathQuill field
mathField.latex(); // => '2^{\\frac{3}{2}}'
```

Check out our [Getting Started Guide](http://docs.mathquill.com/en/latest/Getting_Started/) for setup instructions and basic MathQuill usage.

## Docs

Most documentation for MathQuill is located on [ReadTheDocs](http://docs.mathquill.com/en/latest/).

Some older documentation still exists on the [Wiki](https://github.com/mathquill/mathquill/wiki).

## Open-Source License

The Source Code Form of MathQuill is subject to the terms of the Mozilla Public
License, v. 2.0: [http://mozilla.org/MPL/2.0/](http://mozilla.org/MPL/2.0/)

The quick-and-dirty is you can do whatever if modifications to MathQuill are in
public GitHub forks. (Other ways to publicize modifications are also fine, as
are private use modifications. See also: [MPL 2.0 FAQ](https://www.mozilla.org/en-US/MPL/2.0/FAQ/))
