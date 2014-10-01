---
category: Users
path: '/user/me/api_key'
title: 'ApiKey'
type: 'GET'

layout: nil
---

Request the ApiKey for the currently authenticated User.

### Request

* The request must be authenticated either by including a **valid [AccessToken](#/post-access-token)** or by using a [Basic Auth Header](http://en.wikipedia.org/wiki/Basic_access_authentication#Client_side).

#### Possible Headers

Token Header

    Authentication: bearer YOUR_ACCESS_TOKEN

Basic Auth Header

    Authorization: Basic YOUR_BASIC_AUTH_CREDENTIALS

The credentials to use for [Basic Auth](http://en.wikipedia.org/wiki/Basic_access_authentication#Client_side) are your Email and Password. You can sign up for an account at [PieceMeta.com](http://www.piecemeta.com) to obtain these credentials.

### Response

Returns an ApiKey object.

#### Body

    {
        key: String,
        secret: String
    }

For errors responses, see the [response status codes](#/response-status-codes).