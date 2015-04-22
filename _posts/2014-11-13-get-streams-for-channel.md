---
category: Packages
path: '/channels/:uuid/streams'
title: 'Get Streams'
type: 'GET'

layout: nil
---

Retrieve a list of available [Streams](#/get-stream) for a [Channel](#/get-channel).

### Request

* **:id** must be an existing [Channel](#/get-channel) UUID.
* Anonymous requests are allowed.

### Response

Returns an array of Stream objects but does not send the actual frame data for each stream. To get the data, use the GET method for particular [Streams](#/get-stream).

#### Body

    [
        {
            uuid: String,
            channel_uuid: String,
            title: String,
            group: String,
            fps: Number,
            created_at: Date,
            updated_at: Date
        }
    ]

For errors responses, see the [response status codes](#/response-status-codes).