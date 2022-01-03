# selector property

Allows you to inject code based on HTML tag, CSS Class, or HTML property. Most of the time you will want to use selector as an HTML tag

eg:

CSS Class
```typescript

@Component({
	selector: '.app-servers'
	...
})

```

HTML property 
```typescript

@Component({
	selector: '[app-servers]'
	...
})

```

HTML tag
```typescript

@Component({
	selector: 'app-servers'
	...
})

```