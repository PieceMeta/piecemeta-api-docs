---
category: Streams
path: '/streams/:uuid'
title: 'Get meta'
type: 'GET'

layout: nil
---

Retrieve a [Stream](#/get-stream)'s descriptive data only.

### Request

* **:uuid** must be an existing Stream id.
* Anonymous requests are allowed.

### Response

Returns a Stream object with the data frames filtered out.

* **frames** is sent as an array of floats.

#### Body

    {
        uuid: String,
        channel_uuid: String,
        title: String,
        group: String,
        fps: Number,
        created_at: Date,
        updated_at: Date
    }

For errors responses, see the [response status codes](#/response-status-codes).