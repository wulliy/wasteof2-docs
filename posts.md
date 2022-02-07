Gets a post.

`GET /posts/60c4d33f1ea77fed94251ab7`

Gets all of the comments of a post per page.

`GET /posts/60c4d33f1ea77fed94251ab7/comments?page=1`

Gets all of the replies of a comment per page.

`GET /comments/60c4d33f1ea77fed94251ab7/replies?page=1`

Makes a new post with any text you input.

Requirements:
- post should only contain `["p", "b", "strong", "i", "em", "u", "s", "li", "ul", "ol", "mark", "code", "blockquote", "pre", "img", "#text"]`
- image src should only be from `["api.wasteof.money", "u.cubeupload.com", "i.ibb.co"]`

`POST /posts`

Edits a post. Requires token in `Authorization` header.

`PUT /posts/60c4d33f1ea77fed94251ab7`

`BODY {post: "new content string"}`

Deletes any post of yours.

`DELETE /posts/60c4d33f1ea77fed94251ab7`

Deletes any comment of a post of yours.

`DELETE /comments/60c4d33f1ea77fed94251ab7/`

Pins any post of yours

`POST /posts/60c4d33f1ea77fed94251ab7/pin`

Unpins any post of yours

`POST /posts/60c4d33f1ea77fed94251ab7/unpin`

Reports any post on wasteof (gets reported)

`POST /posts/612b7b3f1148ae87a61ab063/report`

`BODY {type: "none", reason: "reasoning on why you fondly find this post so horrendous that you had to report it so the admins could take care of it."}`

Loves / Unloves any post on wasteof

`POST /posts/612b7b3f1148ae87a61ab063/love`

See if an user loved a post or not

`GET /posts/612b7b3f1148ae87a61ab063/loves/jeffalo`

Reposts an post

`POST /posts`

`BODY {post: "<p>hello world</p>", "repost": "612e01a8e5d5662da8e66306"}`
