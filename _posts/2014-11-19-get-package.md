---
category: Packages
path: '/packages/:uuid'
title: 'Get'
type: 'GET'

layout: nil
---

Retrieve a Package.

### Request

* **:uuid** must be an existing Package UUID.
* Anonymous requests are allowed.

### Response

Returns a Package object.

#### Body

    {
        uuid: String,
        user_uuid: String,
        title: String,
        description: String,
        created_at: Date,
        updated_at: Date
    }

For errors responses, see the [response status codes](#/response-status-codes).