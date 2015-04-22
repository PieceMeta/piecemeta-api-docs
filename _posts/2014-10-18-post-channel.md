---
category: Channels
path: '/channels/:id'
title: 'Create'
type: 'POST'

layout: nil
---

Create a new Channel for a Package.

### Request

* **The body can't be empty** and must at least include a valid [package_uuid](#/get-package) and a title.
* **package_uuid** must be an existing [Package](#/get-package) UUID that you own.
* You can create a hierarchy of channels by setting **parent_channel_uuid** to an existing Channel UUID within a [Package](#/get-package) you own.
* The headers must include a **valid [AccessToken](#/post-access-token)**.

#### Body

    {
        package_uuid: String,
        title: String,
        parent_channel_uuid: String
    }

### Response

Returns a Package object.

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