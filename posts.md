Gets a post.

`GET /posts/60c4d33f1ea77fed94251ab7`

Gets all of the comments to a post per page.

`GET /posts/60c4d33f1ea77fed94251ab7/comments?page=1`

Gets all of the replies to a comment per page.

`GET /comments/60c4d33f1ea77fed94251ab7/replies?page=1`

Makes a new post with any text you input.

Requirements:
- Your post should only contain `["p", "b", "strong", "i", "em", "u", "s", "li", "ul", "ol", "mark", "code", "blockquote", "pre", "img", "#text"]`
- The image src should only be from `["api.wasteof.money", "u.cubeupload.com", "i.ibb.co"]`
- `#text` is the content inside an element and it is also a [shadow DOM element](https://web.dev/shadowdom-v1/)

Optional:
- Adding in a `repost` argument, followed with a post id allows you to repost posts

`POST /posts`

Edits a post. Requires your token in the `Authorization` header.

```
PUT /posts/60c4d33f1ea77fed94251ab7
BODY {post: "new content string"}
```

Deletes any post of yours.

`DELETE /posts/60c4d33f1ea77fed94251ab7`

Deletes any comment in a post of yours.

`DELETE /comments/60c4d33f1ea77fed94251ab7`

Pins any post of yours.

`POST /posts/60c4d33f1ea77fed94251ab7/pin`

Unpins any post of yours.

`POST /posts/60c4d33f1ea77fed94251ab7/unpin`

Reports any post.

```
POST /posts/612b7b3f1148ae87a61ab063/report
BODY {type: "none", reason: "they took my lunch money"}
```

Loves / Unloves any post on wasteof2.

`POST /posts/612b7b3f1148ae87a61ab063/love`

See if an user loved a post or not.

`GET /posts/612b7b3f1148ae87a61ab063/loves/jeffalo`

Reposts an post. (The `repost` argument must be a vaild post ID)

```
POST /posts
BODY {post: "<p>hello world</p>", "repost": "612e01a8e5d5662da8e66306"}
```
