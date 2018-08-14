# Timber Backend

Proposed API routes:

## login/
Self explanatory, takes `email, hash`

## user/

### /me
Returns personal data, takes `session_token`

### /<id>
Returns public user data, takes `id`

#### /match
Matches with user, takes `id`

## /nearby
Returns nearby matches, takes `coordinates`

