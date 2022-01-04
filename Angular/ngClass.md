# ngClass

Property [[Directive]] that triggers a CSS class depending on a conditional value. The directive also takes a key value pair compared to ngStyle

1. Class Name
2. Condition when it should be turned on 

eg: 

```css
.online {
	color: white;
}
```
Online is defined in component logic:
`[ngClass]="{online: serverStatus === 'online'}"`

Or source the logic to a method

`[ngClass]="{online: serverIsOnline()}"`