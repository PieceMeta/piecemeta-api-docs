---
category: Channels
title: 'Export'
path: '/export/channels/:id.:format'
type: 'GET'

layout: nil
---

A complete version of a data Channel with it's Streams included.

### Request

* **:id** must be an existing [Channel](#/get-channel) id.
* Anonymous requests are allowed.

The **:format** must be one of the following:

* JSON: `.json
* MessagePack: `.msgpack`
* XML: `.xml`
* CSV: `.csv`

### Response

Sets the Content-Type for the response and returns a file in the requested format.
