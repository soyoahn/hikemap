---
layout: page
---
Last Updated: 2024-06-22

# Add a trail `POST` 

Creates a new [`trails`](trails.html) resource in the Hikemap service.

The request body must include all attributes for the new trail.

## URL
`{server_url}/trails`

## Request headers
Accept all default headers in Postman.

| Header Parameter |  Value | Description |
| -------------- | ------ | ------------ |
| Accept | application/json | **Required.** This is the expected response data type.|

## Request body

Specify a JSON representation of the [`trails`](trails.html) object.

All properties are required.

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `name` | string | Display name of hiking trail |
| `city` | string | City name |
| `state` | string | 2-letter U.S. state code (example: `CA`) |
| `difficulty` | string | Difficulty rating. <br>Values can be: `Easy`, `Medium`, `Difficult`, or `Very Difficult` |
| `length` | number | Length of trail in miles (mi) |
| `elevation_gain` | number | Total elevation gain for the trail in feet (ft) |
| `description` | string | Short description of the trail |
| `image_url` | string | Full web url |

## Request body example
Method: `POST` | Request body: Raw JSON

💡 **Note:** The unique `id` property will be generated for the new object when the POST request is successful.

```
    {
      "name": "Mt. Astley",
      "city": "Miami",
      "state": "FL",
      "difficulty": "Very Diffcult",
      "length": 3,
      "elevation_gain": 9001,
      "description": "Never gonna give you up. Never gonna let you down.",
      "image_url": "https://www.giantfreakinrobot.com/wp-content/uploads/2022/08/rick-astley.jpg"
    }  
```

## Response body example
```
    {
      "id": "e848",
      "name": "Mt. Astley",
      "city": "Miami",
      "state": "FL",
      "difficulty": "Very Diffcult",
      "length": 3,
      "elevation_gain": 9001,
      "description": "Never gonna give you up. Never gonna let you down.",
      "image_url": "https://www.giantfreakinrobot.com/wp-content/uploads/2022/08/rick-astley.jpg"
    }
```

## Response codes

| Status | Return status | Description |
| ------------- | ----------- | ----------- |
| 201 | Created | The request has been fulfilled and resulted in a new resource being created. |
| 400 | Bad Request | Check your URL syntax and your request headers. <br>In Postman, use default headers. |
| 500 | Internal Server Error | Unexpected error. Check your request body for typos.  |
