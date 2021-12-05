# curried function

Function that returns a function that takes the return value from the previous function.
```javascript
const add = (x, y) => x + y
add(2, 3) //=> 5
```

Here it is again in curried form …

```javascript
const add = x => y => x + y
```

Here is the same1 code without arrow functions …

```javascript
const add = function (x) {
  return function (y) {
    return x + y
  }
}
```