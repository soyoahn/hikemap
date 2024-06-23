---
layout: page
---
Last Updated: 2024-06-22

# Get trails by attributes like `name` or `state`

Endpoint: {base_url}/**[trails](trails.html)**

Before you begin: 
* Be sure you've completed the first tutorial: [Set up your development environment](tutorial-getting-started.html)
* Start the server: 
```
    cd <your GitHub repo workspace>/hikemap/json-db
    .\start-server.bat
 ```

## By name
> [!IMPORTANT]
> You must URL encode `name` values.

For example for the `Half Dome` value, use `Half%20Dome`.

### URL syntax: 
{server_url}/trails?**name**=*<name_value>* 

Example:
```
curl http://localhost:3000/trails?name=Half%20Dome
```

## By state

### URL syntax: 
{server_url}/trails?**state**=*<state_value>* 

Example:
```
curl http://localhost:3000/trails?state=WA
```