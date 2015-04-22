---
category: Packages
path: '/packages/:uuid/channels'
title: 'Get Channels'
type: 'GET'

layout: nil
---

Retrieve a list of available [Channels](#/get-channel) for a [Package](#/get-package).

### Request

* **:uuid** must be an existing [Package](#/get-package) UUID.
* Anonymous requests are allowed.

### Response

Returns an array of Channel objects.

#### Body

    [
        {
            uuid: String,
            package_uuid: String,
            title: String,
            parent_channel_uuid: String,
            created_at: Date,
            updated_at: Date
        }
    ]

For errors responses, see the [response status codes](#/response-status-codes).