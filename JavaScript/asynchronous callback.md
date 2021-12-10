# asnychronous callback

This is a snippet to deal with asynchronous work (especially through built-ins that don't use the [[Promise]] API) through the use of a [[Callback Function]], eg:

```javascript
function firstFunction(_callback){
    // do some asynchronous work
    // and when the asynchronous stuff is complete
    _callback();    
}

function secondFunction(){
    // call first function and pass in a callback function which
    // first function runs when it has completed
    firstFunction(function() {
        console.log('huzzah, I\'m done!');
    });    
}
```

Or using ES6

`firstFunction(() => console.log('huzzah, I\'m done!'))`