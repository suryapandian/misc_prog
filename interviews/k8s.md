### Task: Build a Kubernetes RBAC filtering API

## Description: 

Design and implement a RESTful API that filters defined Kubernetes RBAC roles and cluster roles, that are bound to given Subject names.

## Requirements:

- API should accept request payload containing details necessary to perform search and filtering.
- Subject names to be provided as a string, a regex pattern, or combination thereof.
- API should allow filtering by any combination of subjects (User, Group, Service account).
- API response should be in the format specified by the caller. Possible options: JSON, YAML.
- The API should run as a Kubernetes application.

## Outcome:

- Return body to include ordered Subjects and their respective Roles and Cluster Roles. The order is specified by the caller, with one of the following options: 
    - Alphabetically
    - Object name string length.

You might also want to consider how to publish such API in a secure way, and representing how the API could accommodate for future changes and be backward compatible. 

# Deliverables might include: 
- Architecture / Design sketches / docs
- API implementation
- Sample resources for deployment of the project

## Notes:

We don’t expect you to spend more than 1-2 days on the technical problem. Your solution, even if not 100% complete, will be taken into consideration and if successful you will be invited to present your solution to us in a face to face / virtual meeting

This solution is for you to work through the problem and present back to us not necessarily needing it to be a complete solution as long as you set the context right, and explain your approach to the problem.

This technical test is not only about measuring that you can code but also about whether you can think for yourselves and break the problem down, or even simplify it a bit if that's what works for you.

it’s about how you frame the solution and what steps you make to solve the problem the best you can.

The IN / OUT from the API is really trivial and the API may be built in a variety of ways, this is down to you to decide how :)

## Company
Appnia
