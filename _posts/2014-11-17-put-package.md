---
category: Packages
path: '/packages/:uuid'
title: 'Update'
type: 'PUT'

layout: nil
---

Update an existing Package.

### Request

* **:uuid** must be an existing Package UUID that you own.
* The headers must include a **valid [AccessToken](#/post-access-token)**.
* Optional attributes are listed below.

#### Body

    {
        title: String,
        description: String
    }

### Response

Returns the updated Package object.

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