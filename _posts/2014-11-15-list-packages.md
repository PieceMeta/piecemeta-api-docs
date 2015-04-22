---
category: Packages
path: '/packages'
title: 'List'
type: 'GET'

layout: nil
---

Retrieve a list of available Packages.

### Request

* Anonymous requests are allowed.

### Response

Returns an array of Package objects.

#### Body

    [
        {
            uuid: String,
            user_uuid: String,
            title: String,
            description: String,
            created_at: Date,
            updated_at: Date
        }
    ]

For errors responses, see the [response status codes](#/response-status-codes).