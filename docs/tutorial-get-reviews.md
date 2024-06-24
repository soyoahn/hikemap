---
layout: page
---
Last Updated: 2024-06-22

# Get reviews by `trail_name` or `username`

Gets an existing [`reviews`](reviews.html) resource in the Hikemap service.

You can use URL parameters in your request to narrow results returned by the server. This tutorial covers the most useful parameters for searching reviews: by trail and by user.

### Before you begin
* Complete the starting tutorial: [Set up your development environment](tutorial-getting-started.html)
* Start the server: 
```
    cd <your GitHub repo workspace>/hikemap/json-db
    .\start-server.bat
 ```

## Get reviews by trail name

💡**Important:** You must URL encode `trail_name` values. Example: For the `Half Dome` value, use `Half%20Dome`.

### URL Parameter: `trail_name`

`{server_url}/reviews?trail_name=<trail_name_value>`

### Request example
Method: `GET`

```
curl http://localhost:3000/reviews?trail_name=Half%20Dome
```

## Get reviews by username

### URL parameter: `username`
`{server_url}/reviews?username=<username_value>`

### Request example
Method: `GET` 

```
curl http://localhost:3000/reviews?username=chris_perez
```

## Response codes

| Status | Return status | Description |
| ------------- | ----------- | ----------- |
| 200 | OK | The request has been fulfilled successfully. |
| 400 | Bad Request | Check your URL syntax and your request headers. <br>In Postman, use default headers. |
| 404 | Not Found | This resource does not exist. |