---
swagger: "2.0"
info:
  title: AWS OpsWorks API Update My User Profile
  version: 1.0.0
  description: Updates a user's SSH public key.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateMyUserProfile:
    get:
      summary: ' Update My User Profile '
      description: Updates a user's SSH public key
      operationId: updateMyUserProfile
      parameters:
      - in: query
        name: SshPublicKey
        description: The user's SSH public key
        type: string
      responses:
        200:
          description: OK
      tags:
      - users
definitions: []
x-collection-name: AWS OpsWorks
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