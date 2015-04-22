---
category: Channels
path: '/channels/:uuid'
title: 'Get'
type: 'GET'

layout: nil
---

Retrieve a Package.

### Request

* **:uuid** must be an existing Channel UUID.
* Anonymous requests are allowed.

### Response

Returns a Channel object.

#### Body

    {
        uuid: String,
        package_uuid: String,
        title: String,
        parent_channel_uuid: String,
        created_at: Date,
        updated_at: Date
    }

For errors responses, see the [response status codes](#/response-status-codes).