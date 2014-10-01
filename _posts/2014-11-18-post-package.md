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
* You can set the **reference_package_id** to extend it's data with the new package.
* You can not be the owner of the **reference_package_id**. Add Channels and Streams to your Packages directly.

#### Body

    {
        title: String,
        description: String,
        reference_package_id: String
    }

### Response

Returns a Package object.

#### Body

    {
        id: String,
        reference_package_id: String,
        user_id: String,
        title: String,
        description: String,
        created_at: String,
        updated_at: String
    }

For errors responses, see the [response status codes](#/response-status-codes).