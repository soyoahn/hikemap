---
layout: page
---
Last Updated: 2024-06-22

# Remove a user `DELETE` 

Removes an existing [`users`](users.html) resource in the Hikemap service.
The request URL must end with the unique `id` of the user resource you intend to delete from the database.

## URL
`{server_url}/users/<id_value>`

## Request headers
Accept all default headers in Postman.

| Header Parameter |  Value | Description |
| -------------- | ------ | ------------ |
| Accept | application/json | **Required.** This is the expected response data type.| 

## Request body
None.

## Request example (URL)
```
http://localhost:3000/users/2
```

## Response codes

| Status | Return status | Description |
| ------------- | ----------- | ----------- |
| 200 | OK | The request has been fulfilled and the requested resource has been deleted. |
| 400 | Bad Request | Check your request headers. |
| 404 | Not Found | This user resource does not exist. |