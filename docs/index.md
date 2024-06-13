---
layout: page
---
![Sign showing icons of two hikers](images/hiking.webp)
# Overview
Track favorite hiking trails and discover new trails based on location and difficulty.

# Features
Users can add hikes with the following attributes:
* Name of hike
* Description
* Location (City/State)
* Difficulty Level (Easy, Medium, Hard)
* Length (Miles)
* Elevation Gain (Feet)
* Image (URL)

Users can rate hikes on a 1 (worst) to 5 (best) rating scale and add a short review.

We collect the following information about users:
* Name
* Email address

# Getting Started
To run a few basic CRUD functions, all you need is a Github account and the following programs installed:
* Github Desktop
* Postman
* Json-server and cURL

💡**Try it out!** Get lists of hikes, users, and reviews by querying our sample database in the following tutorials:

* [Tutorial: Getting Started](tutorial-gettingstarted.html)

The sample database used in these tutorials is [hikemap-db.json](../json-db/hikemap-db.json).

# Developing interactions with hikes, reviews, and users
Use our tutorials to understand how to access these core resources: 
* Hikes
    * Add a new hike
    * Update attributes on an existing hike
* Users
    * Add a user
    * Remove a user
* Reviews
    * Add a review
    * Add an attribute on an existing review

## API reference docs
Detailed descriptions of the service's resources.

The API reference docs refer to a `{base_url}` when they
refer to the URL of a resource. The `{base_url}` value depends
on the installation of the service.

When running a local test, the `{base_url}` is
typically `http://localhost:3000`.

* [user resource](ADD)
* [review resource](ADD)
* [trail resource](ADD)