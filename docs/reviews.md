---
layout: page
---
Last Updated: 2024-06-22

# `reviews` resource

## Endpoint

```shell
{server_url}/reviews
```

Contains trail reviews submitted by users.

## Resource properties

Sample `reviews` resource:

```js
    {
      "id": "1",
      "trail_name": "Mount Si",
      "user_id": "1",
      "username": "john_doe",
      "rating": 5,
      "comment": "Amazing hike! Highly recommend."
    },
```

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `id` | integer | Unique numeric ID  |
| `trail_name` | string | Display name of hiking trail |
| `user_id` | integer | ID of the [users](users.html) resource |
| `username` | string | Display name that can be composed of letters, numbers, and underscores |
| `rating` | integer | Rating ranging from 1 (worst) to 5 (best) |
| `comment` | string | User's review of this hike |

## Operations

The `reviews` resource supports the following operations.

* [Get reviews by trail name or username](tutorial-get-reviews.html) `GET`
* [Edit a review](tutorial-update-review.html) `PUT`
