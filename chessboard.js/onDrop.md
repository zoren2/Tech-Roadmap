# onDrop

An event that fires when a piece is dropped. If `snapback` is returned from the function, the piece will return to its source square.
If `trash` is returned from the function, the piece will be removed. (Useful for board editing)

#Arguments 
1. Source of the dragged piece.
2. Target of the dragged piece
3. Actual piece selected
4. New position once piece is dropped
5. Old position before the piece was picked up
6. Current board orientation