# Recursive DOM Traversal
Here's a "canonical" way of traversing the DOM.

```html
<div id="subtree">
	<form>
		<input type = "text">
	</form>
	<p>Paragraph</p>
	<span>Span</span>
</div>
```

The following JS will recursively traverse these HTML elements.
(For an extra exercise, visualize the tree created in the DOM by this HTML.)

```javascript
function traverseDOM(element, callback) {
	// In the context of this problem the entry node is first passed
	// into the traverseDOM function. 
	callback(element); 
	// This function then uses the passed in assert method which asks
	element = element.firstElementChild;
	while (element) // It's not boolean I'm guessing if it's not undefined... Also it will eventually be false in which it will get popped off the call stack, probably one of the "leaf" items from the recursive calls.
	{
		traverseDOM(element, callback);
		element = element.nextElementSibling; // Hmm it needs to know about implementing what's happening from the callback function...
	}
}
```

