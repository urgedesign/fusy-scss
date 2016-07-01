Fusy SCSS
===========================

This is a [Foundation](http://foundation.zurb.com)-style grid framework based on [Susy](http://susy.oddbird.net).
It uses Susy's math to output a configurable set of grid classes that mimics the Foundation grid.
Currently supported are _row_, _columns_, _push_ and _pull_ classes.


Documentation
-------------


Define your grid settings:
```scss
$total-columns: 	12; 						// The number of columns in your grid
$column-gutter:		0.125; 						// The size of a gutter in relation to a single column (e.g. 0.125 = 1/8th)
$column-width:		80px; 						// The width of a single column (px)
$container-width: 	1440px;						// Sets a max-width for the container (px)
```


Adjust breakpoints if required:
```scss
$small-range: 		(0rem, 40rem);
$medium-range: 		(40.063rem, 64rem);
$large-range: 		(64.063rem, 90rem);
$xlarge-range: 		(90.063rem, 120rem);
$xxlarge-range: 	(120.063rem);
```


Configure which classes to output
```scss
$include-small: 	true;
$include-medium: 	true;
$include-large: 	true;
$include-xlarge: 	false;
$include-xxlarge: 	false;
```

Usage
-----

Once you've configured the grid and compiled the SCSS you can use [grid classes identical to Foundation](http://foundation.zurb.com/sites/docs/grid.html), eg.
```
<div class="row">
    <div class="small-6 medium-5 large-2 columns">
        ...
    </div>
    <div class="small-6 medium-7 large-10 columns">
        ...
    </div>
</div>
```

Limitations
-----------
Currently supported are _row_, _columns_, _push_ and _pull_ classes.
_-only_ classes are currently omitted.
