---
category: Channels
path: '/channels/:id'
title: 'Delete'
type: 'DELETE'

layout: nil
---

Delete an existing Channel.

### Request

* **:id** must be an existing Channel id that you own.
* The headers must include a **valid [AccessToken](#/post-access-token)**.

### Response

Returns the deleted Channel.

#### Body

    {
        id: String
        package_id: String,
        title: String,
        parent_channel_id: String,
        created_at: Date,
        updated_at: Date
    }

For errors responses, see the [response status codes](#/response-status-codes).