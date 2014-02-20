*This repository is a mirror of the [component](http://component.io) module [javve/get-by-class](http://github.com/javve/get-by-class). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/javve-get-by-class`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
![web component logo](http://i49.tinypic.com/e7nj9v.png)

# getByClass

A cross-browser implementation of getElementsByClass.
Heavily based on [Dustin Diaz](https://github.com/ded)'s function: [http://dustindiaz.com/getelementsbyclass](http://www.dustindiaz.com/getelementsbyclass).

Uses default `getElementsByClassName` if it's available.

## Component
Built to be used with the [Component package manager](https://github.com/component/component). Read more here:
* [Component at Github](https://github.com/component/component)
* [TJ Holowaychuk's introduction](http://tjholowaychuk.com/post/27984551477/components)

## Installation

    $ component install javve/get-by-class

## Example

```js
var getByClass = require('get-by-class');

var menu = document.getElementById('menu');

// Returns set of items
var activeItem = getByClass(menu, 'active');

// Returns single item
var activeItem = getByClass(menu, 'active', true);
```

## API

### getByClass(container, className, single)

Find all elements with class `className` inside `container`.  
Use `single = true` to increase performance in older browsers
when only one element is needed.

## License

  MIT
