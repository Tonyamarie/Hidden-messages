# Hidden-messages
What do I use to unhide hidden messages in the development??  Like this one....                 function assert(condition,opt_message){if(!condition){var message="Assertion failed";if(opt_message)message=message+": "+opt_message;var error=new Error(message);var global=function(){return this}();if(global.traceAssertionsForTesting)console.warn(error.stack);throw error}return condition}function assertNotReached(opt_message){assert(false,opt_message||"Unreachable code hit")}function assertInstanceof(value,type,opt_message){if(!(value instanceof type)){assertNotReached(opt_message||"Value "+value+" is not a[n] "+(type.name||typeof type))}return value}
