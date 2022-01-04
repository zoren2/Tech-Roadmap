# ngIf

Angular [[Directive]] to control the DOM.

It can be enhanced by [else] condition for example to render another template.

eg:

```typescript
<p *ngIf="serverCreated; else noServer">
	Server was created, server name is {{serverName}}
	<ng-template #noServer>
		<p> No server was created! </p>
	</ng-template>
</p>
	