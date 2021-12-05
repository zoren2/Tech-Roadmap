# Callback Function

A callback function is passing a function as an argument to another function that mihgt at a later point in application execution, call the passed-in function. This tends to be very useful for things like [[event handlers]].

- Whenever we setup a function to be called at a later time, you're then setting up a [callback].

```

var text = "Domo arigato!";
report("Before defining functions"); // Adds a styled <p> element

function useless(ninjaCallback) {
	report("In useless function")
	return ninjaCallback();
}

function getText() {
	report("In getText function");
	return text;
}

report("Before making all the calls");

// This line prints if true, else it adds a line through the middle of the text
assert(useless(getText) === text, "The useless function works! " + text);

report("After the calls have been made");

```

getText gets passed into useless as a function

```
function useless(ninjaCallback) // getText function "becomes" ninjaCallback
```