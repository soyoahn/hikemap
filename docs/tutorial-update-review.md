---
layout: page
---
Last Updated: 2024-06-22

# Edit a review `PUT` 

Updates an existing [`reviews`](reviews.html) resource in the Hikemap service. 

The request URL must end with the unique `id` of the `reviews` resource you intend to modify in the database.

Important: The request body must include all properties in the `reviews` object and not just the ones intended for update.

## URL
`{server_url}/reviews/<id_value>`

## Request headers
Accept all default headers in Postman.

| Header Parameter |  Value | Description |
| -------------- | ------ | ------------ |
| Accept | application/json | **Required.** This is the expected response data type.|

## Request body

Specify a JSON representation of the [`reviews`](reviews.html) object.

All properties are required, though you might want to constrain users' options to only update `rating` and `comment`.

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `trail_name` | string | Display name of the trail, matching the `name` property in the [trails](trails.html) resource |
| `user_id` | integer | ID of the [users](users.html) resource |
| `username` | string | Display name that can be composed of letters, numbers, and underscores |
| `rating` | integer | Rating ranging from 1 (worst) to 5 (best) |
| `comment` | string | User's review of this hike |

## Request body example
Method: `PUT` | Request body: Raw JSON
```
  {
      "trail_name": "Mount Si",
      "user_id": "1",
      "username": "john_doe",
      "rating": 3,
      "comment": "Edit: 3 months later, still great! Amazing hike! Highly recommend."
  }
```

## Response codes

| Status | Return status | Description |
| ------------- | ----------- | ----------- |
| 200 | OK | The request has been fulfilled and resulted in the resource being updated. |
| 400 | Bad Request | Check your URL syntax and your request headers. <br>In Postman, use default headers. |
| 500 | Internal Server Error | Unexpected error. Check the syntax or your request body for typos.  |
