---
category: Streams
path: '/streams/:uuid'
title: 'Update'
type: 'PUT'

layout: nil
---

Update an existing Stream for a Channel within a Package.

* You can group together multiple Streams using the **group** property (e.g. Set **group** to "position" for three Streams with the titles "x", "y" and "z" for spatial data).

### Request

* **:uuid** must be an existing Stream UUID.
* The headers must include a **valid [AccessToken](#/post-access-token)**.
* **The body can't be empty** and must at least include a valid [channel_uuid](#/get-channel), title, frames (array of floats) and fps (frames per second).

#### Body

    {
        channel_uuid: String,
        title: String,
        group: String,
        data_frames: [Number],
        frame_duration: Number
    }

### Response

Returns a Stream object.

* **frames** is expected to be an array of floats.

#### Body

    {
        uuid: String,
        channel_uuid: String,
        title: String,
        group: String,
        frames: [Number],
        fps: Number,
        created_at: Date,
        updated_at: Date
    }

For errors responses, see the [response status codes](#/response-status-codes).