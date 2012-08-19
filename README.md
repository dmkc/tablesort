# tablesort.js

Tablesort is a small and simple sorting component for tables written in Javascript. It has no dependencies and should have no interference with other libraries.

## Basic usage

``` html
<script src='tablesort.min.js'></script>
<script>
  new Tablesort(document.getElementById('table-id'));
</script>
```

## Features

* Sort strings
* Sort numbers
* Sort currency 
* Basic date sorting: either the `dd/mm/yy` format, or '{month} {day}', 
  e.g. "Sept 25".

## Ender support

Add `tablesort` as an internal chain method to your [Ender](http://ender.no.de) compilation.

    $ ender add tablesort

Use it:

``` js
$('.table').tablesort();
```

## Building

Developers can rebuild the minified library by running:

``` bash
  npm install --dev
  make
```

## TODOs

* Tests
* Pass in an options object to:
  - Choose which row to begin sorting on.
  - Column exclusion
  - EventListener to rebuild the table.
