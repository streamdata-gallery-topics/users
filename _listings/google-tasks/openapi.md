---
swagger: "2.0"
x-collection-name: Google Tasks
x-complete: 1
info:
  title: Tasks
  description: lets-you-manage-your-tasks-and-task-lists-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /tasks/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/@me/lists:
    get:
      summary: Get Users @me Lists
      description: Returns all the authenticated user's task lists.
      operationId: tasks.tasklists.list
      x-api-path-slug: usersmelists-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of task lists returned on one page
      - in: query
        name: pageToken
        description: Token specifying the result page to return
      responses:
        200:
          description: OK
      tags:
      - Users
      - '@me'
      - Lists
    post:
      summary: Add Users @me Lists
      description: Creates a new task list and adds it to the authenticated user's
        task lists.
      operationId: tasks.tasklists.insert
      x-api-path-slug: usersmelists-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
      - '@me'
      - Lists
  /users/@me/lists/{tasklist}:
    delete:
      summary: Delete Users Task List
      description: Deletes the authenticated user's specified task list.
      operationId: tasks.tasklists.delete
      x-api-path-slug: usersmeliststasklist-delete
      parameters:
      - in: path
        name: tasklist
        description: Task list identifier
      responses:
        200:
          description: OK
      tags:
      - Users
      - Task
      - List
    get:
      summary: Get Users Task List
      description: Returns the authenticated user's specified task list.
      operationId: tasks.tasklists.get
      x-api-path-slug: usersmeliststasklist-get
      parameters:
      - in: path
        name: tasklist
        description: Task list identifier
      responses:
        200:
          description: OK
      tags:
      - Users
      - Task
      - List
    patch:
      summary: Patch Users Task List
      description: Updates the authenticated user's specified task list. This method
        supports patch semantics.
      operationId: tasks.tasklists.patch
      x-api-path-slug: usersmeliststasklist-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tasklist
        description: Task list identifier
      responses:
        200:
          description: OK
      tags:
      - Users
      - Task
      - List
    put:
      summary: Put Users Task List
      description: Updates the authenticated user's specified task list.
      operationId: tasks.tasklists.update
      x-api-path-slug: usersmeliststasklist-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tasklist
        description: Task list identifier
      responses:
        200:
          description: OK
      tags:
      - Users
      - Task
      - List
---