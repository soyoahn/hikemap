---
layout: page
---

# Get reviews by trail name

Before you begin, be sure you've done the first tutorial: [Set up your development environment](tutorial-getting-started.html)


## Get 

To test your development system, follow these steps:

1. In a web browser, go to [Hikemap repo](https://github.com/soyoahn/hikemap) and fork the repo. 
2. Open GitHub Desktop and clone the `hikemap` repo to get a local copy on your computer.
3. Open a PowerShell command window and go to the `hikemap/json-db directory`: 

    ```shell
    cd <your GitHub repo workspace>/hikemap/json-db
    ```
2. Start the json server by running start-server.bat: 
    ```shell
    .\start-server.bat
    ``` 
    If your development system is set up correctly, you should see something like the following output: 
    ```shell
    JSON Server started on PORT :3000
    Watching hikemap-db.json...
    Index:
    http://localhost:3000/

    Endpoints:
    http://localhost:3000/trails
    http://localhost:3000/users
    http://localhost:3000/reviews
    ``` 
4. In a new PowerShell window, test a call to the service. Get the first available hiking trail:

    ```shell
    curl http://localhost:3000/trails/1
    ```
    If the service is running correctly, you should see the first sample hike from the service: 

    ```js
    {
    "id": "1",
    "name": "Mount Si",
    "city": "North Bend",
    "state": "WA",
    "difficulty": "Intermediate",
    "length": 8,
    "elevation_gain": 3150,
    "description": "Mount Si is a popular hiking de...
    ```
    **If you get this output, you've completed this tutorial successfully.** You can continue running any other Hikemap tutorial.
    
    If you don't see this output, you must troubleshoot the issue before you can try other tutorials.

    <details>
    <summary><b>Tips for troubleshooting</b></summary>
        
    1. Check your commands for typos
    2. Check that you're in the correct directory
    3. Look up any error messages to verify that all prerequisite software was installed correctly
    4. Check that all prerequisite software is up to date
    </details>
        