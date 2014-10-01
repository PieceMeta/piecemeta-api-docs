---
category: Packages
path: '/packages'
title: 'Create'
type: 'POST'

layout: nil
---

Create a new Package.

### Request

* The headers must include a **valid [AccessToken](#/post-access-token)**.
* **The body can't be empty** and must at least include the title.

#### Body

    {
        title: String,
        description: String
    }

### Response

Returns a Package object.

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