# messages
> TOKEN: your user(bot) token.<br/>MESSAGEIDS: an array of message ids. note that message ids are different than comment ids.
### Get all of your read messages.
```http
GET /messages/read
Authorization: TOKEN
```

### Get all of your unread messages.

```http
GET /messages/unread
Authorization: TOKEN
```

### Get your total message count.

```http
GET /messages/count
Authorization: TOKEN
```

### Mark message(s) as read.

```http
POST /messages/mark/read
Authorization: TOKEN
Content-Type: application/json

{ "messages": MESSAGEIDS }
```

### Mark message(s) as unread.

```http
POST /messages/mark/unread
Authorization: TOKEN
Content-Type: application/json

{ "messages": MESSAGEIDS }
```
