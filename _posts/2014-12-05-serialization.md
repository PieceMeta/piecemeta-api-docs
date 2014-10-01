---
category: General
title: 'Serialization formats'

layout: nil
---

### Choosing a format

Available serialization formats are: [JSON](http://json.org), [MessagePack](http://msgpack.org) and [XML](http://www.w3.org/XML/).

If a format is not applicable to the current request or no format was specified the **default is JSON**

By supplying one of the following MIME types you can choose the format for object serialization in requests and responses.

* JSON: `application/json`
* MessagePack: `application/msgpack`
* XML `application/xml`

Alternatively you can add a file type extension to the URL to set the format.

* JSON: `.json`
* MessagePack: `.msgpack`
* XML: `.xml`

