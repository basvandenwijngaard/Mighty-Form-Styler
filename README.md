# Mighty Form Styler

jQuery Mighty Form Styler replaces you form select element with a html ul list so you can easily and completely style it with css. With some little magic it behaves just like a regular select element.

Version 1.0.1

Requires jQuery 1.7 or newer.

Licensed under:
MIT License - https://github.com/MightyMedia/Mighty-Form-Styler/blob/master/LICENSE.txt

## Requirements

* jQuery 1.7+

## Installation

To use Mighty Form Styler make sure you have jQuery 1.7 or newer. Next, add jquery.mfs.min.js to your webpage.

```html
<script type="text/javascript" src="jquery.mfs.min.js"></script>
```

## Basic usage

### Initialize

```javascript
$(document).ready(function(){
    $('form').mfs();
});
```

### Refresh (e.g. when you updated the values via ajax)

```javascript
$('form').mfs('refresh');
```

### Remove

```javascript
$('form').mfs('destroy');
```

## Options

At this point there are four options available.

### dropdownHandle

Add text or HTML in the dropdown handle (the little arrow down). For example, when you want to use fontawesome icons in the handle.

```javascript
$('form').mfs({
    'dropdownHandle': '<i class="icon-chevron-down"></i>'
});
```

### enableScroll

Enable a scrollbar in the dropdown list, as default this is set to _false_.

```javascript
$('form').mfs({
    'enableScroll' : true
});
```

### maxHeight

Set the max height in pixels for the dropdown list, as default this is set to _200_. The setting *enableScroll* needs to be set to _true_ for this setting to have effect.

```javascript
$('form').mfs({
    'enableScroll' : true,
    'maxHeight'    : 150
});
```

### autoWidth

Make dropdown list width adjust to widest option

```javascript
$('form').mfs({
    'autoWidth' : true
});
```

## Demo

You can preview a live demo at: http://www.binkje.nl/mfs/

## Issues

If you have any ideas or bugs, please submit them to the GitHub issue tracker at https://github.com/MightyMedia/Mighty-Form-Styler/issues.