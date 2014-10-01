---
category: Channels
path: '/channels/:id'
title: 'Get'
type: 'GET'

layout: nil
---

Retrieve a Package.

### Request

* **:id** must be an existing Channel id.
* Anonymous requests are allowed.

### Response

Returns a Channel object.

#### Body

    {
        id: String,
        package_id: String,
        title: String,
        parent_channel_id: String,
        created_at: Date,
        updated_at: Date
    }

For errors responses, see the [response status codes](#/response-status-codes).