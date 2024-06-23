---
layout: page
---
Last Updated: 2024-06-22

# Get reviews by `trail_name` or `username`

Endpoint: {base_url}/**[reviews](reviews.html)**

Before you begin: 
* Be sure you've completed the first tutorial: [Set up your development environment](tutorial-getting-started.html)
* Start the server: tutorial-get-trail-by-name-or-state
```
    cd <your GitHub repo workspace>/hikemap/json-db
    .\start-server.bat
 ```

## Get reviews by trail name
💡<span style="color:orange">**Important:**</span> You must URL encode `trail_name` values.

For example for the `Half Dome` value, use `Half%20Dome`.

### URL syntax: 
{server_url}/reviews?**trail_name**=*<trail_name_value>*  

Example:
```
curl http://localhost:3000/reviews?trail_name=Half%20Dome
```

## Get reviews by username

### URL syntax: 
{server_url}/reviews?**username**=*<username_value>*

Example:
```
curl http://localhost:3000/reviews?username=chris_perez
```