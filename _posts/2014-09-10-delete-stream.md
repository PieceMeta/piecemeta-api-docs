---
category: Streams
path: '/streams/:uuid'
title: 'Delete'
type: 'DELETE'

layout: nil
---

Delete an existing Stream.

### Request

* **:uuid** must be an existing Stream id that you own.
* The headers must include a **valid [AccessToken](#/post-access-token)**.

### Response

Returns the deleted Stream.
    
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