# jQuery Persistent Form Values #

Any element made persistant with jQuery-persist will store its value in a cookie when changed - and when returning to the page later, retrieve its values from that cookie. By default, it uses the fields name to identify its persisted value, so it will work across different forms and pages. Use the 'context' option to differentiate between different forms that use inputs with the same name.

Example usage:
```
		$('input,select,textarea').persist(options);
```
options:
```
{ 
	context : 'def',	// a context or namespace for each field
	replace	: true,		// replace existing field contents if any
	cookie	: 'jqpersist',	// cookies basename
	path	: '/',		// cookie path
	domain	: null,		// cookie domain
	expires	: null		// cookie expiry (eg 365)
}
```

Requires jQuery.cookies.
There's a tester/demo included in the download.