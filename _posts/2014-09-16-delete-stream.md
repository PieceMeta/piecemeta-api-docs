---
category: Streams
path: '/streams/:id'
title: 'Delete'
type: 'DELETE'

layout: nil
---

Delete an existing Stream.

### Request

* **:id** must be an existing Stream id that you own.
* The headers must include a **valid [AccessToken](#/post-access-token)**.

### Response

Returns the deleted Stream.
    
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