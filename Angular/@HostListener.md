# @HostListener
A [[directive]] which is declared within a class inside a [Typescript] file (usually name.directive.ts) which listens [event] which occurs on an element that uses custom [[property binding]].

You will need to append official [event]s supported by Angular.
Eg: `@HostListener('mouseenter')`

Use case:

```typescript

@HostListener('mouseenter') mouseover(eventData: Event) {
	this.renderer.setStyle(this.elRef.nativeElement, 'background-color', 'blue', false, false)
}
```

#Tags 
[[directive]]
[[Renderer2]]