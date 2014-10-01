---
category: Streams
path: '/streams:id'
title: 'Get'
type: 'GET'

layout: nil
---

Retrieve a Stream for a Channel within a Package.

### Request

* **:id** must be an existing Stream id.
* Anonymous requests are allowed.

### Response

Returns a Stream object.

* **frames** is sent as an array of floats.

#### Body
    
    {
        id: String,
        channel_id: String,
        title: String,
        group: String,
        frames: [Number],
        fps: Number,
        created_at: Date,
        updated_at: Date
    }

For errors responses, see the [response status codes](#/response-status-codes).