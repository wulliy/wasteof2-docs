Get user's profile and information

`GET /users/jeffalo`

Get user's followers. (You can get the amount of followers through the `stats.followers` key)

`GET /users/jeffalo/followers`

Get the users that a certain user is following. (You can get the amount of people that the user is following through the `stats.following` key)

`GET /users/jeffalo/following`

See if a user is following another user.

`GET /users/jeffalo/followers/jeffolo`

Gets a user's profile picture.

`GET /users/jeffalo/picture`

Gets a user's banner. (Shows blank if no banner set)

`GET /users/wasteof.money/banner`

Gets a user's posts per page.

`GET /users/jeffalo/posts?page=1`

Gets the name of an user?

`GET /users/jeffalo/name`

Gets the feed of an user

`GET /users/jeffalo/following/posts`

Follow a user.

`POST /users/jeffalo/followers`

Set a bio. Could've done a `/users/bio` though, but oh well.

`PUT /users/jeffalo/bio`

Sets a new username for you. As long as it's not taken.

`PUT /users/jeffalo/name`

Creates a new user.

`POST /users`

Sets a new profile picture. Must be an image!

`PUT /users/jeffalo/picture`
