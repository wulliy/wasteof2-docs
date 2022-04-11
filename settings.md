It's pretty self-explanatory.

`GET /settings`

Deletes the Github authentication method

`DELETE /settings/auth/github`

Deletes the Google authentication method

`DELETE /settings/auth/google`

Deletes the password authentication method

`DELETE /settings/auth/password`

Sets a new password of your choice (Make sure to remember your new password!)

`PUT /settings/auth/password`

Enables/Disables the Github authentication method

`POST /settings/auth/github/enable` - `POST /settings/auth/github/disable`

Enables/Disables the Google authentication method

`POST /settings/auth/google/enable` - `POST /settings/auth/google/disable`

Enables/Disables the Password authentication method

`POST /settings/auth/password/enable` - `POST /settings/auth/password/disable`

Hides the recovery message at the top of the page

`POST /settings/hide-recovery-message`

Removes the recovery email you set

`DELETE /settings/email`

Sets a recovery email for your account. If one has already been set, you can change it instead

`PUT /settings/email`

Sends an email to reset a user's password

`POST /settings/password-reset`
