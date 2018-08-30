---
swagger: "2.0"
x-collection-name: BlazeMeter
x-complete: 0
info:
  title: Blazemeter Get User Register
  description: Get user register.
  version: 1.0.0
host: a.blazemeter.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/active/sessions:
    get:
      summary: Get User Active Sessions
      description: Get user active sessions.
      operationId: active_sessions
      x-api-path-slug: useractivesessions-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Active
      - Sessions
  /user/active/terminate:
    post:
      summary: Post User Active Terminate
      description: Post user active terminate.
      operationId: panic_terminate
      x-api-path-slug: useractiveterminate-post
      parameters:
      - in: body
        name: blazemeter\Routing\v4\UserModel5
        description: session_ids (required)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Active
      - Terminate
  /user/collections:
    get:
      summary: Get User Collections
      description: Get user collections.
      operationId: retrieveCollections
      x-api-path-slug: usercollections-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: skip
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Collections
  /user/invites:
    get:
      summary: Get User Invites
      description: Get user invites.
      operationId: retrieveInvites
      x-api-path-slug: userinvites-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Invites
  /user/locations:
    get:
      summary: Get User Locations
      description: Get user locations.
      operationId: retrieveLocations
      x-api-path-slug: userlocations-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Locations
  /user/masters:
    get:
      summary: Get User Masters
      description: Get user masters.
      operationId: retrieveMasters
      x-api-path-slug: usermasters-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: skip
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Masters
  /user/password:
    patch:
      summary: Patch User Password
      description: Patch user password.
      operationId: user.password.patch
      x-api-path-slug: userpassword-patch
      parameters:
      - in: body
        name: blazemeter\Routing\v4\UserModel1
        description: currentPassword (required)newPassword (required)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Password
    post:
      summary: Post User Password
      description: Post user password.
      operationId: user.password.post
      x-api-path-slug: userpassword-post
      parameters:
      - in: body
        name: blazemeter\Routing\v4\UserModel3
        description: currentPassword (required)newPassword (required)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Password
    put:
      summary: Put User Password
      description: Put user password.
      operationId: user.password.put
      x-api-path-slug: userpassword-put
      parameters:
      - in: body
        name: blazemeter\Routing\v4\UserModel2
        description: currentPassword (required)newPassword (required)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Password
  /user/projects:
    get:
      summary: Get User Projects
      description: Get user projects.
      operationId: retrieveProjects
      x-api-path-slug: userprojects-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Projects
  /user/register:
    get:
      summary: Get User Register
      description: Get user register.
      operationId: register_retrieve
      x-api-path-slug: userregister-get
      parameters:
      - in: query
        name: email
        description: Email address
      - in: query
        name: firstName
        description: First name
      - in: query
        name: lastName
        description: Last name
      - in: query
        name: password
        description: Password
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Register
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