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

## Request body example (JSON)
💡 **Note:** The unique `id` will be generated when the POST  request is successful.
```
    {
      "name": "Wildwood Canyon Loop",
      "city": "Burbank",
      "state": "CA",
      "difficulty": "Intermediate",
      "length": 2,
      "elevation_gain": 672,
      "description": "Popular for running and hiking, this is a dog-friendly hike with areas of shade throughout the trail, and a vista of Los Angeles at the summit.",
      "image_url": "https://www.burbankca.gov/documents/67263/652332/012621+-+PR+-+Wildwood+Park+%285%29.jpg"
    }  
```

## Response codes

| Status | Return status | Description |
| ------------- | ----------- | ----------- |
| 201 | Created | The request has been fulfilled and resulted in a new resource being created. |
| 400 | Bad Request | Check your request headers. |
| 500 | Internal Server Error | Unexpected error. Check your request body for typos.  |
