---
layout: page
---

# Hikemap REST API Overview
 The Hikemap API provides the following resources: `trails`, `reviews`, and `users`.
 
 For details about hikemap's features, see [About Hikemap](about.html).

# Getting Started
To run a few basic CRUD functions on the Hikemap service, all you need is a GitHub account and the basic software needed to run cURL commands with json-server.

💡**Try it out!** Follow this tutorial to get the required software and make your first Hikemap API call to our sample database:
* [Set up your development environment](tutorial-getting-started.html)

# Tutorials
The sample database used in these tutorials is [hikemap-db.json](https://github.com/soyoahn/hikemap/blob/main/json-db/hikemap-db.json).

After completing the tutorial under Getting Started, use these further tutorials to understand how to do GET, POST, PUT, and DELETE methods on these resources:
* Trails
    * [Get trails by attribute](tutorial-get-trails-by-attribute.html) `GET`
    * [Add a trail](tutorial-new-trail.html) `POST`
* Reviews
    * [Get reviews by trail name or username](tutorial-get-reviews.html) `GET`
    * [Edit a review](tutorial-update-review.html) `PUT`
* Users
    * [Remove a user](tutorial-delete-user.html) `DELETE`

Note: Although we don't tutorials available for each CRUD function across all resource types, those functions _are_ supported on all resources.

# Reference
Hikemap API has the following resources: 
* [Trails resource](trails.html)
* [Reviews resource](reviews.html)
* [Users resource](users.html)

Last Updated: 2024-06-22