#jQuery-Breakpoints.js

**Simple breakpoint events for responsive JS.**

###Define your breakpoints (*desktop is set by default*):

```
$( window ).breakpoints( {
	breakpoints : { 
		'mobile' : 640,
		'mini-tablet' : 1024,
		'tablet' : 1280
	}
} );
```

###Subscribe to a breakpoint event:

```
$( window ).on( 'breakpointChange', function( e, data ) {
	console.log( 'Active Breakpoint: ' + data.activeBreakpoint );
	console.log( 'Deactivated Breakpoint: ' + data.deactivatedBreakpoint );
} );
```

It's literally that simple.