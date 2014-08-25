# Bootstrap Dual List Box

## Synopsis

Bootstrap Dual List Box is a dual list box implementation especially designed for Bootstrap and jQuery. This control is
quite easy for users to understand and use. Also it is possible to work with very large multi-selects without confusing
the user.

## Usage

First off you should create a simple `<select id="some-name">` tag. After which you can initialize the dual list box
as a jQuery plugin like so: `$('some-name').DualListBox();`. There are also some options associated with this plugin.

## Options / API

There are currently two ways to use this component. First up is by using html5 `data-*` attributes embedded in the
select tag, but you can also provide a Javascript Object. The variable names are the same all around and can be even
mixed and matched within the select or Javascript. The current options are: 

| Option       | Type    | Default    | Description |
| ------------ | ------- | ---------- | ----------- |
| `json`       | Boolean | true       | Whether to download the data via a JSON request.  |
| `uri`        | URI     | local.json | The relative or absolute URI where to receive the data from. | 
| `value`      | String  | id         | This determines what JSON field is handled as the value. |
| `text`       | String  | name       | This determines what JSON field is handled as the text. | 
| `title`      | String  | Example    | The title of the control. |
| `horizontal` | Boolean | false      | Whether the control is lay out horizontal or vertical. |
| `timeout`    | UInt    | 500        | Timeout when to start searching with the filter. |
| `textLength` | UInt    | 45         | Maximum text length of when the element should contain title-attributes. |
| `moveAllBtn` | Boolean | true       | Whether to display the move all button (from left to right or vice-versa). |
| `maxAllBtn`  | UInt    | 500        | Integer to determine from which length to display the warning message below. |
| `warning`    | String  | <...>      | Warning message that is displayed when trying to move large amounts of elements. |

## [Demo](http://geodan.github.io/duallistbox/index.html)

Small demo that shows the functionality of the plugin. 

## Installation

Copy the `dual-list-box.js` file to a directory in your project and reference it via Javascript. After which it should
be available as a jQuery plugin. 

## Tested compatibility

Currently the plugin is confirmed working in:

* Internet Explorer 9+
* Mozilla Firefox (latest)
* Google Chrome (latest)

Other browsers are currently untested, but should work when they are compatible with jQuery. 

## License

```
The MIT License (MIT)

Copyright (c) 2014 Geodan B.V. (Alex van den Hoogen)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```