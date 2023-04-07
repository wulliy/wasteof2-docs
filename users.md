Gets a user's profile and information.

`GET /users/jeffalo`

Gets a user's followers. (You can get the amount of followers through the `stats.followers` key)

`GET /users/jeffalo/followers`

Get the users that a certain user is following. (You can get the amount of people that the user is following through the `stats.following` key)

`GET /users/jeffalo/following`

See if a user is following another user.

`GET /users/jeffalo/followers/jeffolo`

Gets a user's profile picture. (If the user doesn't exist, it will return a generated SVG profile picture instead)

`GET /users/jeffalo/picture`
`GET /users/jeffalo/picture?optimized=true`

Gets a user's banner. (Appears blank if no banner was set)

`GET /users/wasteof.money/banner`
`GET /users/wasteof.money/banner?optimized=true`

Gets a user's posts per page.

`GET /users/jeffalo/posts?page=1`

Gets the name of a user?

`GET /users/jeffalo/name`

Gets the feed of a user.

`GET /users/jeffalo/following/posts`

Follows a user.

`POST /users/jeffalo/followers`

Sets a bio.

`PUT /users/jeffalo/bio`

Sets a new username for you. As long as it's available.

`PUT /users/jeffalo/name`

Creates a new user.

`POST /users`

Sets a new profile picture. Must be an image!

`PUT /users/jeffalo/picture`
