# Chessboard.js

Javascript library to render board and pieces using common web browsers.

The drag events take certain `return` values in order to achieve certain behavior

eg:  [[onDrop]] example

```javascript
 var onDrop = function(source, target) {

 // see if the move is legal

 var move = game.move({

 from: source,

 to: target,

 promotion: document.getElementById("promote").value

 });

  

 // illegal move

 if (move === null) return 'snapback';

  

 prepareMove();

 };
```