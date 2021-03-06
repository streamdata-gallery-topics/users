---
swagger: "2.0"
x-collection-name: Azure API Management
x-complete: 0
info:
  title: Azure API Management API Users Get
  description: Gets the details of the user specified by its identifier.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/groups/{groupId}/users
  : get:
      summary: GroupUsers ListByGroups
      description: Lists a collection of the members of the group, specified by its
        identifier.
      operationId: GroupUsers_ListByGroups
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamegroupsgroupidusers-get
      parameters:
      - in: query
        name: $filter
        description: '| Field            | Supported operators    | Supported functions               ||------------------|------------------------|-----------------------------------||
          id               | ge, le, eq, ne, gt, lt | substringof, contains, startswith,
          endswith || firstName        | ge, le, eq, ne, gt, lt | substringof, contains,
          startswith, endswith || lastName         | ge, le, eq, ne, gt, lt | substringof,
          contains, startswith, endswith || email            | ge, le, eq, ne, gt,
          lt | substringof, contains, startswith, endswith || state            | eq                     |
          N/A                               || registrationDate | ge, le, eq, ne,
          gt, lt | N/A                               || note             | ge, le,
          eq, ne, gt, lt | substringof, contains, startswith, endswith |'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Group Users
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/groups/{groupId}/users/{uid}
  : put:
      summary: GroupUsers Create
      description: Adds a user to the specified group.
      operationId: GroupUsers_Create
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamegroupsgroupidusersuid-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Group Users
    delete:
      summary: GroupUsers Delete
      description: Remove existing user from existing group.
      operationId: GroupUsers_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamegroupsgroupidusersuid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Group Users
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/users:
    get:
      summary: Users ListByService
      description: Lists a collection of registered users in the specified service
        instance.
      operationId: Users_ListByService
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusers-get
      parameters:
      - in: query
        name: $filter
        description: '| Field            | Supported operators    | Supported functions               ||------------------|------------------------|-----------------------------------||
          id               | ge, le, eq, ne, gt, lt | substringof, contains, startswith,
          endswith || firstName        | ge, le, eq, ne, gt, lt | substringof, contains,
          startswith, endswith || lastName         | ge, le, eq, ne, gt, lt | substringof,
          contains, startswith, endswith || email            | ge, le, eq, ne, gt,
          lt | substringof, contains, startswith, endswith || state            | eq                     |
          N/A                               || registrationDate | ge, le, eq, ne,
          gt, lt | N/A                               || note             | ge, le,
          eq, ne, gt, lt | substringof, contains, startswith, endswith |'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/users/{uid}
  : get:
      summary: Users Get
      description: Gets the details of the user specified by its identifier.
      operationId: Users_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameusersuid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
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