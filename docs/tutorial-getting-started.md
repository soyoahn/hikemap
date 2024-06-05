---
layout: page
---

# Set up your dev environment

These steps assume you're on a supported version of Microsoft Windows and supported versions of the following software installed:
* [GitHub Desktop](https://desktop.github.com)
    * You'll need a [GitHub account](https://github.com)
* [Node.js](https://nodejs.org/en/)
* [json-server](https://www.npmjs.com/package/json-server)
* [Postman](https://www.postman.com/downloads/)
* [PowerShell](https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell?view=powershell-7.4)

## Test your development system

To test your development system, follow these steps:

1. In a web browser, go to https://github.com/soyoahn/hikemap and fork the hikemap repo. 
2. Open GitHub Desktop and clone the hikemap repo to get a local copy on your computer.
3. Open a PowerShell command window and go to the `hikemap/json-db directory`: 

    ```shell
    cd <your GitHub repo workspace>/hikemap/json-db
    ```
2. Start the json server by running start-server.bat: 
    ```shell
    .\start-server.bat
    ``` 
3.  Check that your development system is set up correctly. You should see something like the following output: 
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
    You must succeed here before you can continue with any other tests or actions on Hikemap. If you don't see this output, troubleshoot the error before attempting  other tutorials.
    
    Tips for troubleshooting: 
    1. Check your commands for typos
    2. Check that you're in the correct directory
    3. Look up any error messages to verify that all prerequisite software was installed correctly
    4. Check that all prerequisite software is up to date
    
    **If you see first hiking trail from the service, you're ready to continue with any of our other tutorials.**
