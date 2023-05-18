# session

> TOKEN: the token of your account, to be used to authorize your bot to make actions on its own behalf.

## FetchAPI example

```js
// create token
let token = await fetch('https://api.wasteof.money/session', { method: "POST", body: JSON.stringify({ username, password }), headers: { Content-Type: "application/json"} }).then(res=>res.json()).then(data => data.token)

// get user associated with token
let user = await fetch('https://api.wasteof.money/session', { headers: { Authorization: token }}).then(res => res.json()).then(console.log)

// invalidate token (logout)
await fetch('https://api.wasteof.money/session', { method: "DELETE", headers: { Authorization: token }).then(res = res.json()).then(console.log)
```

### Get the current logged in user's session.

```http
GET /session`
Authorization: TOKEN
```

### Log you into an account.
> It is recommended to only do this once, then continue to use that token, because as of writing this, tokens never expire.
```http
POST /session

{ username: string, password: string }
```
#### Returns (if valid)
```json
{ token: TOKEN }
```

### Invalidate your TOKEN.
> Do this if you plan on regenorating a new token every time you run the bot.

```http
DELETE /session
Authorization: TOKEN
```
