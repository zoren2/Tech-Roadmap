# Directive

Informally Directives are instructions in the DOM level. Think of [[component]]s with a template or an HTML property you can control with a custom [directive] or built-in [directive] which controls whether the element renders or not.

eg: A Custom Directive example

`<p appTurnGreen> Receives Green Background! </p>` 

```typescript
@Directive({
	selector:'[appTurnGreen]'
})

export class TurnGreenDirective {
 //...
}
```
### Built-In Directives
#Element - needs a * 
[[ngIf]], [ngFor] 

#Property
[[ngStyle]], [[ngClass]]

