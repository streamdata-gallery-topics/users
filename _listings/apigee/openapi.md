---
swagger: "2.0"
x-collection-name: Apigee
x-complete: 1
info:
  title: Apigee Edge
  description: restful-management-api-to-create-configure-and-manage-api-proxies-and-api-products-create-and-manage-apps-and-app-developers-and-more-
  version: 1.0.0
host: api.enterprise.apigee.com
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users:
    get:
      summary: Get Users
      description: Gets a list of users.
      operationId: getUsers
      x-api-path-slug: users-get
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: Post Users
      description: Creates a user.
      operationId: postUsers
      x-api-path-slug: users-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{user_email}:
    get:
      summary: Get Users User Email
      description: Gets a user.
      operationId: getUsersUserEmail
      x-api-path-slug: usersuser-email-get
      parameters:
      - in: path
        name: user_email
        description: Mention the user email
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Email
    post:
      summary: Post Users User Email
      description: Updates a user.
      operationId: postUsersUserEmail
      x-api-path-slug: usersuser-email-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      - in: path
        name: user_email
        description: Mention the user email
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Email
    delete:
      summary: Delete Users User Email
      description: Deletes a user.
      operationId: deleteUsersUserEmail
      x-api-path-slug: usersuser-email-delete
      parameters:
      - in: path
        name: user_email
        description: Mention the user email
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Email
  /users/{user_email}/userroles:
    get:
      summary: Get Users User Email Userroles
      description: Gets roles for a user.
      operationId: getUsersUserEmailUserroles
      x-api-path-slug: usersuser-emailuserroles-get
      parameters:
      - in: path
        name: user_email
        description: Mention the user email
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Email
      - Userroles
    post:
      summary: Post Users User Email Userroles
      description: Associates a user with a organizational user role.
      operationId: postUsersUserEmailUserroles
      x-api-path-slug: usersuser-emailuserroles-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      - in: path
        name: user_email
        description: Mention the user email
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Email
      - Userroles
  /userroles/{role_name}/users:
    get:
      summary: Get Userroles Role Name Users
      description: Lists users for a role.
      operationId: getUserrolesRoleNameUsers
      x-api-path-slug: userrolesrole-nameusers-get
      parameters:
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Userroles
      - Role
      - Users
    post:
      summary: Post Userroles Role Name Users
      description: Adds user to role.
      operationId: postUserrolesRoleNameUsers
      x-api-path-slug: userrolesrole-nameusers-post
      parameters:
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Userroles
      - Role
      - Users
  /userroles/{role_name}/users/{user_email}:
    get:
      summary: Get Userroles Role Name Users User Email
      description: Checks user in a given system role
      operationId: getUserrolesRoleNameUsersUserEmail
      x-api-path-slug: userrolesrole-nameusersuser-email-get
      parameters:
      - in: path
        name: role_name
        description: Mention the role name
      - in: path
        name: user_email
        description: Mention the user email
      responses:
        200:
          description: OK
      tags:
      - Userroles
      - Role
      - Users
      - User
      - Email
    delete:
      summary: Delete Userroles Role Name Users User Email
      description: Deletes user for a role.
      operationId: deleteUserrolesRoleNameUsersUserEmail
      x-api-path-slug: userrolesrole-nameusersuser-email-delete
      parameters:
      - in: path
        name: role_name
        description: Mention the role name
      - in: path
        name: user_email
        description: Mention the user email
      responses:
        200:
          description: OK
      tags:
      - Userroles
      - Role
      - Users
      - User
      - Email
  /users/{user_email}/userroles/{role_name}:
    delete:
      summary: Delete Users User Email Userroles Role Name
      description: Deletes organizational role for a user.
      operationId: deleteUsersUserEmailUserrolesRoleName
      x-api-path-slug: usersuser-emailuserrolesrole-name-delete
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: query
        name: org
        description: Specify the organization name
      - in: path
        name: role_name
        description: Mention the role name
      - in: path
        name: user_email
        description: Mention the user email
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Email
      - Userroles
      - Role
  /users/{user_name}/permissions:
    get:
      summary: Get Users User Name Permissions
      description: Gets permissions for a user at global level
      operationId: getUsersUserNamePermissions
      x-api-path-slug: usersuser-namepermissions-get
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: query
        name: path
        description: Specify the resource path
      - in: path
        name: user_name
        description: Mention the user name
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Permissions
  /users/{user_email}permissions/get:
    get:
      summary: Get Users User Email Permissions Get
      description: Checks user has particular permission for a resource at global
        level
      operationId: getUsersUserEmailPermissionsGet
      x-api-path-slug: usersuser-emailpermissionsget-get
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: query
        name: path
        description: Specify the resource path
      - in: query
        name: userEmail
        description: Mention the user name
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Emailpermissions
      - Get
---