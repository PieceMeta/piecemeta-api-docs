---
category: Streams
path: '/streams/:uuid'
title: 'Get frames'
type: 'GET'

layout: nil
---

Retrieve a [Stream](#/get-stream)'s frames only.

### Request

* **:uuid** must be an existing Stream UUID.
* Anonymous requests are allowed.

### Response

Returns a Stream object with all descriptive fields filtered out.

* **frames** is sent as an array of floats.

#### Body

    {
        uuid: String,
        channel_uuid: String,
        frames: [Number]
    }

For errors responses, see the [response status codes](#/response-status-codes).