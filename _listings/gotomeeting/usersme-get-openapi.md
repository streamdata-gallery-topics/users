---
swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 0
info:
  title: SCIM Get Current User
  description: Queries the identity of the current authenticated user.
  termsOfService: https://developer.citrixonline.com/terms-use
  contact:
    name: Developer Support
    url: https://developer.citrixonline.com
    email: developer-support@citrixonline.com
  version: N/A
host: api.citrixonline.com
basePath: /identity/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Schemas/Users:
    get:
      summary: Get User Schema
      description: Queries the user schema. The user schema is defined in SCIM Core
        Schema (http://www.simplecloud.info/specs/draft-scim-core-schema-01.html#resource-schema).
      operationId: getUserSchema
      x-api-path-slug: schemasusers-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Schemas
      - Users
  /Users:
    get:
      summary: Get Users
      description: Queries multiple user identities in the organization domain. Filtering
        is available.
      operationId: getUsers
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: filter
        description: Without a filter, all users in a user domain are returned
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: Create User
      description: Creates a new organization user and adds them to the user domain.
        The user email domain must match an existing organization email domain.
      operationId: createUsers
      x-api-path-slug: users-post
      parameters:
      - in: body
        name: body
        description: The details of the user to create
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
  /Users/me:
    get:
      summary: Get Current User
      description: Queries the identity of the current authenticated user.
      operationId: getMe
      x-api-path-slug: usersme-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
      - Me
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---