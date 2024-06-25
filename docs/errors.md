---
layout: page
---

# Hikemap error codes
Common issues behind the error codes.

| Status | Return status | Description | Notes |
| ------------- | ----------- | ----------- | ----------- |
| 200 | OK | The request has been fulfilled successfully. | Success on `GET` `PUT` `DELETE` |
| 201 | Created | The request has been fulfilled and resulted in a new resource being created. | Success on `POST` |
| 400 | Bad Request | Check your URL syntax and your request headers. <br>In Postman, use default headers. | Typically caused by typos in your request or missing request headers. |
| 404 | Not Found | This resource does not exist. | Happens when you make a legitimate request to access or delete an object that doesn't exist. |
| 500 | Internal Server Error | Unexpected error. Check the syntax or your request body for typos. | For all other errors. |