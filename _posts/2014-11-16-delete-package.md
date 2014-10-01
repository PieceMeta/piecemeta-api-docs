---
category: Packages
path: '/packages/:id'
title: 'Delete'
type: 'DELETE'

layout: nil
---

Delete an existing Package.

### Request

* **:id** must be an existing Package id that you own.
* The headers must include a **valid [AccessToken](#/post-access-token)**.

### Response

Returns the deleted Package.

#### Body

    {
        id: String,
        user_id: String,
        title: String,
        description: String,
        created_at: String,
        updated_at: String
    }

For errors responses, see the [response status codes](#/response-status-codes).