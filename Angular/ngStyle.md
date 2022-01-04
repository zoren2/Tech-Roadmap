# ngStyle
Built-in property [[Directive]] in order to control element styling. The right hand side takes an JSON object with key value pairs. First is style then value is style property.

Basic Use With Camel Casing:

```typescript

<p [ngStyle]="{backgroundColor: getColor()}" >
	
	</p>
<!-- getColor is an unimplemented method to grab color from the component logic --!>

```

Example with single quote:

```typescript

<p [ngStyle]="{'background-color': getColor()}" >
	
	</p>
<!-- getColor is an unimplemented method to grab color from the component logic --!>

```
