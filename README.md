# C# Authentication HTTP Requests 
## Create a complete webapi using Jwt Authentication 

## Learning Objectives
- Use a bearer token to protect an API resource

## Introduction

In this exercise, you're going to build a small but complete bearer token authentication system. Here's a reminder for the flow:

1. The client sends a request containing login credentials to the server.
2. The server checks the credentials are correct and sends back a token.
3. The client sends a request to a secure resource, putting the token in the `authorization` header of the request.
4. The server verifies that the token is valid and sends back the requested resource, or an error message if the token wasn't valid.

Here's the diagram again to help you visualise this flow:

![](./assets/Auth_Flow.png)

### Core Criteria
You will need to:

-install relevant dependencies when required e.g. BCrypt or simlar for encrypting passwords in your database
-add relevent configuration to the appsettings.json e.g. ElephantSql instance / token
-add an endpoint which handles the Registration / Login 
-add entities, request/response models, db context, repository and any other classes you wish 
-keep code clean and comment where applicable using xml comments


### Extension Criteria
You should complete all of the above plus:

-add an endpoint which returns data from your database and ensure the endpoint method is decorated with 
the Authorize to secure it
-if you wish to explore roles e.g. [Authorize(Role="Administrator")] then feel free



