---
category: General
title: 'Authentication'

layout: nil
---

### Public resources

Listed are all actions available to non-authenticated users:

* `GET` [List packages](#/list-packages)
* `GET` [Get package](#/get-package)
* `GET` [List channels](#/list-channels)
* `GET` [Get channel](#/get-channel)
* `GET` [List streams](#/list-streams)
* `GET` [Get stream](#/get-stream)
* `GET` [Get exports](#/get-exports)
* `GET` [Get public user profile](#/get-user)

### Authenticated Requests

To be able to make authenticated requests you need to

* create an account at [PieceMeta.com](http://www.piecemeta.com)
* either look up your credentials there or [get your ApiKey](#/get-api-key) through the API
* request an [AccessToken](#/post-access-token)

You can then add the required Authentication header to your requests to perform authenticated requests.

    Authentication: bearer YOUR_ACCESS_TOKEN
