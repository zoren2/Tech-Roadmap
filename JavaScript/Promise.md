# Promise

A [promise] is a placeholder for a value that we don't have now but will have later, a guarantee that we will eventualy know the result of an asynchronous computation.

```javascript

//Creates a promise by calling a built-in Promise constructor and passing in a callback function with two parameters: resolve and reject

const ninjaPromise = new Promise((resolve, reject) => {

	//A promise is successfully resolved by calling the passed-in resolve function (and rejected by calling the reject function).
	resolve("Hattori");
	//reject("An error resolving a promise!");
} 

ninjaPromise.then(ninja => {
	assert(ninja === "Hattori", "We were promised Hattori!"); },
	err => { fail("There shouldn't be an error")
});

```

If successful the resolve callback is called. Second is called if an error occurs.

Built-in *then* method on the [Promise] object that takes two callback functions.