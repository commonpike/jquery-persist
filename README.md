=jquery-persist 201203*pike=
	
persist form values in localstorage or sessionstorage

example usage:

	$('input,select,textarea').persist(options);
	
	$('input,select,textarea').unpersist(options);
	
options

	context 	: 'def',				// a context or namespace for each field
	replace		: true,					// replace existing field contents if any
	basename	: 'jqpersist',	// storage variable basename
	session		: false					// use sessionstorage instead of localstorage


To debug, try

	console.log(jQuery.persist.keys);
	console.log(jQuery.persist.vals);
