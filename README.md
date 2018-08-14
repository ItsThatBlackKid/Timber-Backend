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
Returns nearby people, takes `coordinates`

## /message
Returns your current messages, takes `id, session_token`

### /message/\<id\>
Sends a message to a user, takes `id, session_token, target_user_id`

# Schemas
*These need to be fleshed out*

- User
- Matches
- Chat, https://stackoverflow.com/questions/39488727/best-way-to-store-chat-messages-in-elasticsearch
I propose for handling the Chat storage and schema we use the ideas presented in the above stackoverflow link for creating a facebook like chat schema using elasticsearch. i have done this before for a similar application and it works nicely. - @phara23

# Notification Channels
- New message
- New match

