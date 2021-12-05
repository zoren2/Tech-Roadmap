# Error Propagation

Using [Promise], you can avoid the [[pyramid of doom]] and [[catch]] the error at the tail end of the promise chain.

```javascript
doSomething()
.then(result => doSomethingElse(result))
.then(newResult => doThirdThing(newResult))
.then(finalResult => console.log(`Got the final result: ${finalResult}`))
.catch(failureCallback);
```