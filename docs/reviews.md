---
layout: page
---
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
      "name": "Mount Si",
      "city": "North Bend",
      "state": "WA",
      "difficulty": "Intermediate",
      "length": 8,
      "elevation_gain": 3150,
      "description": "Mount Si is a popular hiking destination...",
      "image_url": "https://example.com/mount-si.jpg"
    },
```

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `id` | number | Unique numerical ID  |
| `name` | string | Display name of hiking trail |
| `city` | string | City name |
| `state` | string | State name (U.S.) |
| `difficulty` | string | Difficulty rating. Values can be: `Easy`, `Medium`, `Difficult`, and `Extremely Difficult` |
| `length` | number | Length of trail in miles, roundtrip |
| `elevation_gain` | number | Total elevation gain for the trail, roundtrip  |
| `description` | string | Short description of the trail |
| `image_url` | string | Full web url |

## Operations

The `trails` resource supports the following operations.

## READ (GET)

* [Get trail by ID](#resource-properties)
* [Get trail review by user ID](#resource-properties)
* [Get trail review by trail name](#resource-properties)
* [Get task by title](tasks-ref-topic-get-task-by-title)

## CREATE (POST)

* [Create a task](tasks-create-task.md/)

## UPDATE (PUT/PATCH)

* [Update a task with PATCH](update-task-with-patch.md)
