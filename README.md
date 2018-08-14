# Timber Backend

Proposed API routes:

## login/
Self explanatory, takes `email, hash`

## user/

### user/me
Returns personal data, takes `session_token`

#### user/me/matches
Returns all matches, takes `session_token`

### user/\<id\>
Returns public user data, takes `id`

#### user/\<id\>/match
Matches with user, takes `id`

## /nearby
Returns nearby matches, takes `coordinates`

