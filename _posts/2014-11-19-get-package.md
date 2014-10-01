---
category: Packages
path: '/packages/:id'
title: 'Get'
type: 'GET'

layout: nil
---

Retrieve a Package.

### Request

* **:id** must be an existing Package id.
* Anonymous requests are allowed.

### Response

Returns a Package object.

#### Body

    {
        id: String,
        user_id: String,
        title: String,
        description: String,
        created_at: Date,
        updated_at: Date
    }

For errors responses, see the [response status codes](#/response-status-codes).