Updates the message count.

```
event name: updateMessageCount
event arguments: messages<int>
```

Redirects every user to a URL.

```
event name: redirect
event arguments: url<str>
```

Sends a message in the public chat.

```
event name: message
event arguments: content<str>
```

---
The structure of a chat message:
```json
{
	"content": "hello world",
	"from": {
		"beta": true,
		"bio": "bio discoverer & wasteof3 beta tester i guess",
		"history": {
			"joined": 1623504859431
		},
		"id": "60c4b7db3db707d5ec773b40",
		"links": [],
		"name": "willy",
		"permissions": {
			"admin": true,
			"banned": false
		},
		"verified": true
	},
	"time": "2023-03-18T13:19:10.172Z"
}
```
