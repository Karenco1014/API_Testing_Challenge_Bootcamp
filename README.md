# Introduction

Todoist is the productivity tool you need to get work and life organized. Collect tasks, organize projects, and plan your day, in this oportunity .
[![Todoist](https://get.todoist.help/hc/article_attachments/360011665940/Web___Inbox.png "Todoist")](https://get.todoist.help/hc/article_attachments/360011665940/Web___Inbox.png "Todoist")

## Goals

This repository has to goal, fulfill the next points:

1. Your authorization token is saved as an environment variable.
2. Create two folders in your collection, one for Projects and another one for Tasks.
3. Inside the Projects folder there should be the next requests:

- Get all projects.
- Create a new project.
- Get a project.
- Update a project.
- Delete a project.

---

- Get active tasks.
- Create a new task.
- Get an active task.
- Update a task.
- Close a task.
- Reopen a task.
- Delete a task.

4. Create Negative scenarios for each one of the requests.

## Installation:

what will you need to run this repository:

- Download [Postman](https://www.getpostman.com/ "Postman")
- Download [Nodejs](https://nodejs.org/en/ "Nodejs")
- Download [newman ](https://www.npmjs.com/package/newman "newman ")
- Download [Visual Studio Code](https://code.visualstudio.com "Visual Studio Code")
- npm install

# Scripts

`"testsPositiveScenarios"`: "npx newman run './Todoist/Tests/Backend /Collections/Positive_scenarios.postman_collection.json' -e './Todoist/Tests/Backend /EnvVariables /Todoist_Pro.postman_environment.json' -r htmlextra --reporter-htmlextra-export './Todoist/Tests/Backend /Reports'/reporte.html",
` "testsNegativeScenarios"`: "npx newman run './Todoist/Tests/Backend /Collections/Negative_scenarios.postman_collection.json' -e './Todoist/Tests/Backend /EnvVariables /Todoist_Pro.postman_environment.json' -r htmlextra --reporter-htmlextra-export './Todoist/Tests/Backend /Reports'/reporte.html"

Clone the repo into your local machine:
`https://github.com/Karenco1014/Todoist.git`

- cd API_Testing_Challenge_Bootcamp

# HTTP Verbs

| HTTP METHOD | POST             | GET        | PUT                                    | DELETE           |
| ----------- | ---------------- | ---------- | -------------------------------------- | ---------------- |
| CRUD OP     | CREATE           | READ       | UPDATE                                 | DELETE           |
| /tasks      | Create new tasks | List tasks | Bulk update                            | Delete all tasks |
| /tasks/1234 | Error            | Show task1 | If exists, update task1; If not, error | Delete task1     |
