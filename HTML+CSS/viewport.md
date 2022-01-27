# viewport

The browsers [viewport] is the area of the window in which web content can be seen.

This is not the same size as the absolute size of a rendered page, hence need for scrollbars.

Eg: Mobile screen has width:640px, a page renders with a virtual viewport of 980px then it will be shrunk down to fit in 640px space.

This mechanism is not effective in combiation with [[media query]] because if a media query kicks in at 640px or 480px it will never be used.

Keep in mind as of 2021 it is not supported in all web browsers.

### Usage of viewport in meta tags
```html 
<meta name="viewport" content="width=device-width, initial-scale=1">
```

`width` property controls size of the viewport. It can be set to specific pixels eg: `width=600` or the keyword `device-width`.

`initial-scale` controls the zoom level when the page is first loaded.

Alternatively `maximum-scale`, `user-scalable` properties control how users are allowed to zoom in or out.