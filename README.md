# UxSignals Widget

# Alternativ 1

```html
<a href="https://app.uxsignals.com/book/CLIENT_ID">Book et intervju!</a>
```

# Alternativ 2

Ren iframe. Vil alltid vises, også når brukeren allerede har booket intervju

```html
<iframe 
    src="https://app.uxsignals.com/embed/book/CLIENT_ID?userId=asdf123" 
    frameborder="0"
    width="100%"
    style="min-height: 300px; width: 100%;"
    allowtransparency="true"
></iframe>
```


# Alternativ 3

Viser widgeten kun når brukeren ikke allerede har booket intervju og du har ledige slots.

```sh
npm install @uxsignals/client
```

```html
<div id="uxsignals"></div>
```

```js
import uxsignals from '@uxsignals/client'
uxsignals.showWidget({
    id: '#uxsignals',
    // Unique identifier for the User. Can be anything as long as it's unique.
    userId: 'asdf',
    clientId: 'CLIENT_ID',
})
```
