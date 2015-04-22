---
category: Exports
title: 'Export package'
path: '/exports/:uuid.:format'
type: 'GET'

layout: nil
---

A complete version of a package with all data included.

### Request

* **:uuid** must be an existing [Package](#/get-package) UUID.
* Anonymous requests are allowed.

The **:format** must be one of the following:

* JSON: `.json
* MessagePack: `.msgpack`
* XML: `.xml`

### Response

A complete [Package](#/get-package) with all it's [Channels](#/get-channel) and their [Streams](#/get-stream)

Sets the Content-Type for the response and returns a file in the requested format.
