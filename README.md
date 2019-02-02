### stellar.js
---
https://github.com/markdalgleish/stellar.js

```js
$(window).stellar();
$('#main').steller();

$.stellar();

$.steller({
  horizontalOffset: 40,
  verticalOffset: 150
});

$('#gallery').steller({
  scrollProperty: 'transform'
});

$('#gallery').stellar({
  positionProperty: 'transform'
});

$.stellar({
  horizontalScrolling: true,
  verticalScrolling: true,
  horizontalOffset: 0,
  verticalOffsetL 0,
  responsive: false,
  scrollProperty: 'scroll',
  positionProperty: 'position',
  parallexBackgrounds: true,
  parallexElements: true,
  hideDistantElements: true,
  hideElement: function($elem) { $elem.hide(); },
  showElement: function($elem) { $elem.show(); }
});

$.stellar.scrollProperty.margin = {
  getLeft: function($element){
    return parseInt($element.css('margin-left'), 10) * -1;
  },
  getTop: function($element){
    return parseInt($element.css('margin-top'), 10) * -1;
  }
}

$.stellar({
  scrollProperty: 'margin'
});

$.stellar.positionProperty.position = {
  setTop: function($element, newTop, originalTop){
    $element.css('top', newTop);
  },
  setLeft: function($element, newLeft, originalLeft){
    $element.css('left', newLeft);
  }
}

$.stellar({
  positionProperty: 'position'
});

$.stellar.positionProperty.foobar = {
  setPotision: function($element, newLeft, originalLeft, newTop, originalTop){
    (newleft - originalLeft) + 'ps, ' +
    (newTop - originalTop) + 'px, ' +
    '0)');
  }
}
$.stellar({
  positionProperty: 'foobar'
});

```

```
<djv data-stellar-ratio="2">

<div data-teller-background-ratio="0.5">

<div data-stellar-ratio="2"
     data-steller-horizontal-offset="40"
     data-steller-vertical-offset="150"
>

<div data-steller-offset-parent="true">
<div data-steller-offset-parent="true"
     data-steller-horizontal-offset="40"
     data-steller-vertical-offset="150">
```

```sh
bower install jquery.stellar  

npm install
grunt
grunt test
grunt lint
grunt watch
```

