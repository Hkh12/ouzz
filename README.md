# Ouzz
Ouzz is a CSS tool for creating responsive grid systems, or CSS box model classes.
Ouzz is built by Sass, so it's fully customizable.
## Table Of Contents
- [Get Started](#getstarted)
- [Grid system](#gridsystem)
- [CSS box model classes](#boxmodel) (`padding` or `margin` in all directions such as `right` or `top`)
- [Classes for CSS displays](#displays) (like `flex` or `inline-block`)
- [Ouzz in RTL](#rtl)

All of these stuff can be used with media queries.
 <!-- see examples at [Example Page](https://hkh12.github.io/ouzz). (Working on it!) -->
### Get Started
To use ouzz, include the css fils into your `HTML` project:
```html
<link rel="stylesheet" href="ouzz.css">
<!-- if you want the minified one: -->
<link rel="stylesheet" href="ouzz.min.css">
```
And if you need right-to-left CSS, add this to your code:
```html
<link rel="stylesheet" href="rtl/ouzz-rtl.css">
<!-- if you want the minified one: -->
<link rel="stylesheet" href="rtl/ouzz-rtl.min.css">
```
### Grid System
Ouzz has a responsive, powerful grid system. It's built over CSS `media` query, so It's fully supported on all browsers.
Our grid system has classes for specifying the width or offset of columns, on every device. Every thing is into a container, `.oz-container` or `.oz-container-f` (for fluid ones).

See a nice example:
```html
<div class="oz-container">
    <div class="oz-col xs-12 sm-10 sm-fw-1 md-8 md-fw-2 lg-6 lg-fw-5 lg-bw-2">
        very small devices: full width (12/12)
        small devices: 10/12 width and 1/12 forward offset
        medium devices: 8/12 width and 2/12 forward offset
        big devices: 6/12 width and 5/12 forward offset and 2/12 backward offset
    </div>
</div>
```
### Box Model
There are some classes for `margin` and `padding`.

See some examples:
```html
<div class="oz-pr-5em oz-pl-7px oz-pt-3rem oz-pb-0">
    padding-right: 5em
    padding-left: 7px
    padding-top: 3rem
    padding-bottom: 0
</div>
<div class="oz-mr-5em oz-ml-7px oz-mt-3rem oz-mb-0">
    margin-right: 5em
    margin-left: 7px
    margin-top: 3rem
    margin-bottom: 0
</div>
```
### Displays
```html
<span class="oz-d-block">My display is block!</span>
<button class="oz-md-d-block">display: block (in medium devices)</button>
```
### Ouzz in `rtl`
In the `rtl` directory, you will see some CSS files. using them, you can change your columns and make them friendly with rtl pages.
