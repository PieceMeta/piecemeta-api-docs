---
category: Channels
path: '/channels/:uuid'
title: 'Delete'
type: 'DELETE'

layout: nil
---

Delete an existing Channel.

### Request

* **:uuid** must be an existing Channel UUID that you own.
* The headers must include a **valid [AccessToken](#/post-access-token)**.

### Response

Returns the deleted Channel.

#### Body

    {
        uuid: String
        package_uuid: String,
        title: String,
        parent_channel_uuid: String,
        created_at: Date,
        updated_at: Date
    }

For errors responses, see the [response status codes](#/response-status-codes).