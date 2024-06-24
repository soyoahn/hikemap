---
layout: page
---
Last Updated: 2024-06-22

# Get trails by attributes like `name` or `state`

Endpoint: {base_url}/**[trails](trails.html)**

### Before you begin
* Complete the starting tutorial: [Set up your development environment](tutorial-getting-started.html)
* Start the server:
```
    cd <your GitHub repo workspace>/hikemap/json-db
    .\start-server.bat
 ```

## Trails by trail name
💡**Important:** You must URL encode `name` values.

For example for the `Half Dome` value, use `Half%20Dome`.

### URL parameter: `name`
`{server_url}/trails?name=<name_value>`

### Request example
Method: `GET` 
```
curl http://localhost:3000/trails?name=Half%20Dome
```

## Trails by U.S. state

### URL parameter: `state`
`{server_url}/trails?state=<state_value>`

### Request example
Method: `GET` 
```
curl http://localhost:3000/trails?state=WA
```

## Response codes

| Status | Return status | Description |
| ------------- | ----------- | ----------- |
| 200 | OK | The request has been fulfilled successfully. |
| 400 | Bad Request | Check your URL syntax and your request headers. <br>In Postman, use default headers. |
| 404 | Not Found | This resource does not exist. |