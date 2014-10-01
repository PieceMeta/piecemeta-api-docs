---
category: Packages
path: '/packages/:id/channels'
title: 'Get Channels'
type: 'GET'

layout: nil
---

Retrieve a list of available [Channels](#/get-channel) for a [Package](#/get-package).

### Request

* **:id** must be an existing [Package](#/get-package) id.
* Anonymous requests are allowed.

### Response

Returns an array of Channel objects.

#### Body

    [
        {
            id: String,
            package_id: String,
            title: String,
            parent_channel_id: String,
            created_at: Date,
            updated_at: Date
        }
    ]

For errors responses, see the [response status codes](#/response-status-codes).