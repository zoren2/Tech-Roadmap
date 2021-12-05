# let

let indicates that this sentence is going to define a binding. Imagine [[binding]] as tentacles rather than boxes. They grasp them.

Compared to a var, let is [[block]] scoped.

```javascript
   let greeting = "say Hi";
   let times = 4;

   if (times > 3) {
        let hello = "say Hello instead";
        console.log(hello);// "say Hello instead"
    }
   console.log(hello) // hello is not defined
```

In this example, hello will be undefined at the end.

Let variables can be updated but nto re-declared.

However, if the same variable is defined in different scopes, there will be no error: