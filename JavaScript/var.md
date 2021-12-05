# var

```var``` is function scoped when it is declared within a function

They can be re-declared and updated

They are also hoisted which means

```
console.log(greeter);
var greeter = "say hello"
```

will be interpreted as

```
var greeter
console.log(greeter); // greeter is undefined
greeter = "say hello"
```
