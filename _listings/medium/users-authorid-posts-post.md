---
swagger: "2.0"
info:
  title: Medium Create User Post
  description: "Creates a post on the authenticated user\u2019s profile."
  termsOfService: https://medium.com/@feerst/2b405a832a2f
  contact:
    name: Hossain Khan
    url: https://github.com/amardeshbd/medium-api-specification
  version: 1.0.0
host: api.medium.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{authorId}/posts:
    post:
      summary: Create User Post
      description: "Creates a post on the authenticated user\u2019s profile"
      operationId: users.authorId.posts.post
      parameters:
      - in: path
        name: authorId
        description: authorId is the user id of the authenticated user
      - in: body
        name: body
        description: Creates a post for user
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - users
      - author
      - posts
definitions:
  Contibutor:
    properties:
      publicationId:
        description: This is a default description.
        type: get
      role:
        description: This is a default description.
        type: get
      userId:
        description: This is a default description.
        type: get
  ContibutorResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  Post:
    properties:
      canonicalUrl:
        description: This is a default description.
        type: get
      content:
        description: This is a default description.
        type: get
      contentFormat:
        description: This is a default description.
        type: get
      license:
        description: This is a default description.
        type: get
      publishStatus:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
  PostDetails:
    properties:
      authorId:
        description: This is a default description.
        type: get
      canonicalUrl:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      license:
        description: This is a default description.
        type: get
      licenseUrl:
        description: This is a default description.
        type: get
      publishStatus:
        description: This is a default description.
        type: get
      publishedAt:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
      url:
        description: This is a default description.
        type: get
  Publication:
    properties:
      description:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      imageUrl:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      url:
        description: This is a default description.
        type: get
  PublicationResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  User:
    properties:
      id:
        description: This is a default description.
        type: get
      imageUrl:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      url:
        description: This is a default description.
        type: get
      username:
        description: This is a default description.
        type: get
  UserResponse:
    properties: []
x-collection-name: Medium
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