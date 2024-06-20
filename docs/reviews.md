---
layout: page
---
# `trails` resource

Endpoint

```shell
{server_url}/trails
```

Contains hiking trail info and stats.

## Resource properties

Sample `trails` resource

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
| `id` | Number | The ID of the hiking trail |
| `title` | String | The title or short description of the task |
| `description` | String | The long description of the task|
| `due_date` | String | The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format of the date and time the task is due |
| `warning` | Number | The number of minutes relative to the `due_date` to alert the user of the task. This is normally a negative number to alert the user before the `due_date`.|
| `id` | Number | The task's unique record ID |

## Operations

The `task` resource supports these operations.

## READ (GET)

* [Get all tasks _(coming soon)_](#resource-properties)
* [Get task by ID _(coming soon)_](#resource-properties)
* [Get task by user ID _(coming soon)_](#resource-properties)
* [Get task by title](tasks-ref-topic-get-task-by-title)

## CREATE (POST)

* [Create a task](tasks-create-task.md/)

## UPDATE (PUT/PATCH)

* [Update a task with PATCH](update-task-with-patch.md)
