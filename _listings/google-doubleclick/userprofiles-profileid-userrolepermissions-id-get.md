---
swagger: "2.0"
info:
  title: Google Doubleclick API Get User Role Permission
  version: 1.0.0
  description: Gets one user role permission by ID.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /userprofiles/{profileId}/userRolePermissions/{id}:
    get:
      summary: Get User Role Permission
      description: Gets one user role permission by ID
      operationId: dfareporting.userRolePermissions.get
      parameters:
      - in: path
        name: id
        description: User role permission ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - advertising
      - users
      - roles
      - permissions
definitions: []
x-collection-name: Google Doubleclick
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