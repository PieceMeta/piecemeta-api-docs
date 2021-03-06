---
category: Streams
path: '/streams/:uuid'
title: 'Get'
type: 'GET'

layout: nil
---

Retrieve a Stream for a Channel within a Package.

### Request

* **:uuid** must be an existing Stream UUID.
* Anonymous requests are allowed.

### Response

Returns a Stream object.

* **frames** is sent as an array of floats.

#### Body
    
    {
        uuid: String,
        channel_uuid: String,
        title: String,
        group: String,
        frames: [Number],
        fps: Number,
        created_at: Date,
        updated_at: Date
    }

For errors responses, see the [response status codes](#/response-status-codes).