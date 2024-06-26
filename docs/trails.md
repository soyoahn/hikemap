---
layout: page
---
Last Updated: 2024-06-22

# `trails` resource

## Endpoint

```shell
{server_url}/trails
```

Contains info that identifies and defines the hiking trail.

## Resource properties

Sample `trails` resource:

```js
    {
      "id": "1",
      "name": "Mount Si",
      "city": "North Bend",
      "state": "WA",
      "difficulty": "Intermediate",
      "length": 8,
      "elevation_gain": 3150,
      "description": "Mount Si is a popular hiking destination...",
      "image_url": "https://example.com/mount-si.jpg"   
    }
```

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `id` | number | Unique numeric ID |
| `name` | string | Display name of hiking trail |
| `city` | string | City name |
| `state` | string | 2-letter U.S. state code (example: CA) |
| `difficulty` | string | Difficulty rating. <br>Values can be: `Easy`, `Medium`, `Difficult`, or `Very Difficult` |
| `length` | number | Length of trail in miles (mi) |
| `elevation_gain` | number | Total elevation gain for the trail in feet (ft)  |
| `description` | string | Short description of the trail |
| `image_url` | string | Full web url |

## Operations

The `trails` resource supports the following operations:

  * [Get trails by attribute](tutorial-get-trails-by-attribute.html) `GET`
  * [Add a trail](tutorial-new-trail.html) `POST`