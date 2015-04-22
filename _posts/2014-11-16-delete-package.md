---
category: Packages
path: '/packages/:uuid'
title: 'Delete'
type: 'DELETE'

layout: nil
---

Delete an existing Package.

### Request

* **:uuid** must be an existing Package UUID that you own.
* The headers must include a **valid [AccessToken](#/post-access-token)**.

### Response

Returns the deleted Package.

#### Body

    {
        uuid: String,
        user_uuid: String,
        title: String,
        description: String,
        created_at: String,
        updated_at: String
    }

For errors responses, see the [response status codes](#/response-status-codes).