---
layout: page
---
Last Updated: 2024-06-22

# `users` resource

## Endpoint

```shell
{server_url}/users
```

Contains user information.

## Resource properties

Sample `users` resource:

```js
  { 
    "id": "5",
    "username": "chris_perez",
    "email": "chris.perez@example.com"
  }
```

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `id` | number | Unique numerical ID  |
| `username` | string | Display name that can be composed of letters, numbers, and underscores |
| `email` | string | User's unique email address and login ID |

## Operations

The `users` resource supports the following operations.

  * [Remove a user](tutorial-delete-user.html) `DELETE`