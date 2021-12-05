# use strict

Directive in [[ES5]] to indicate that the code should be executed in strict mode. This allows you to use undeclared variables. It is a [[literal expression]].

eg:

- x = 3.14; // This will cause an error because x is not declared.

When declared in a function, it has only local [[scope]].

- function myFunction() {
	"use strict";
	y = 3.14 // This will cause an error 
}

Basically declare everything once you use the directive and consider its scope.

#scope
#variable 
#literal