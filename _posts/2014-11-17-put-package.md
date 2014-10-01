---
category: Packages
path: '/packages/:id'
title: 'Update'
type: 'PUT'

layout: nil
---

Update an existing Package.

### Request

* **:id** must be an existing Package id that you own.
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
        id: String,
        user_id: String,
        title: String,
        description: String,
        created_at: Date,
        updated_at: Date
    }

For errors responses, see the [response status codes](#/response-status-codes).