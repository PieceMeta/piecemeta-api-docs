---
category: Packages
path: '/packages/:package_id/channels/:id/streams'
title: 'Get Streams'
type: 'GET'

layout: nil
---

Retrieve a list of available [Streams](#/get-stream) for a [Channel](#/get-channel) within a [Package](#/get-package).

### Request

* **:id** must be an existing [Channel](#/get-channel) id.
* **:package_id** must be an existing [Package](#/get-package) id.
* Anonymous requests are allowed.

### Response

Returns an array of Stream objects but does not send the actual frame data for each stream. To get the data, use the GET method for particular [Streams](#/get-stream).

#### Body

    [
        {
            id: String,
            channel_id: String,
            title: String,
            group: String,
            fps: Number,
            created_at: Date,
            updated_at: Date
        }
    ]

For errors responses, see the [response status codes](#/response-status-codes).