# UxSignals Widget

# Alternativ 1

```html
<a href="https://app.uxsignals.com/book/CLIENT_ID">Book et intervju!</a>
```

# Alternativ 2

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
    userInfo: {
        email: 'users@email.com',
    }
})
```
