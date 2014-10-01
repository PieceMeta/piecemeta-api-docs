---
category: Channels
path: '/channels/:id'
title: 'Create'
type: 'POST'

layout: nil
---

Create a new Channel for a Package.

### Request

* **The body can't be empty** and must at least include a valid [package_id](#/get-package) and a title.
* **package_id** must be an existing [Package](#/get-package) id that you own.
* You can create a hierarchy of channels by setting **parent_channel_id** to an existing Channel id within a [Package](#/get-package) you own.
* The headers must include a **valid [AccessToken](#/post-access-token)**.

#### Body

    {
        package_id: String,
        title: String,
        parent_channel_id: String
    }

### Response

Returns a Package object.

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