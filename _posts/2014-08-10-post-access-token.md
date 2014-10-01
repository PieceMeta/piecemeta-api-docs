---
category: Users
path: '/user/me/tokens'
title: 'AccessToken'
type: 'POST'

layout: nil
---

Request an access token with your [ApiKey](#/get-api-key) credentials to be able to perform [authenticated requests](#/authentication).

* The token is valid for 60 days from it's issue date.

Sign up for an account at [PieceMeta.com](http://www.piecemeta.com) to obtain your credentials.

### Request

* **The body can't be empty** and must include your valid [ApiKey](#/get-api-key) credentials.

#### Body

    {
        key: String,
        secret: String
    }

### Response

Sends back an AccessToken object. If the current token is expired a new one is created automatically.

#### Body

    {
        user_id: String,
        token: String,
        issued: Date,
        hours_valid: Number
    }

For errors responses, see the [response status codes](#/response-status-codes).