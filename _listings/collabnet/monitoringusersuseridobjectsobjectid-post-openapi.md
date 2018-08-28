---
swagger: "2.0"
x-collection-name: CollabNet
x-complete: 0
info:
  title: CollabNet TeamForge API Documentation Monitors the current object for the
    given userid.
  version: 1.0.0
  description: Monitors the current object for the given userid..
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /monitoring/users/{userid}/objects/{objectid}:
    get:
      summary: Monitoring the current object or not for the given user id (true /
        false)
      description: Monitoring the current object or not for the given user id (true
        / false).
      operationId: isObjectMonitoredByUserid
      x-api-path-slug: monitoringusersuseridobjectsobjectid-get
      parameters:
      - in: path
        name: objectid
        description: Object id
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Current
      - Object
      - Notthe
      - Given
      - User
      - (true
      - ""
      - ""
      - False)
    post:
      summary: Monitors the current object for the given userid.
      description: Monitors the current object for the given userid..
      operationId: monitorObjectByUserid
      x-api-path-slug: monitoringusersuseridobjectsobjectid-post
      parameters:
      - in: path
        name: objectid
        description: Object id
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - Monitors
      - Current
      - Objectthe
      - Given
      - Userid
  /monitoring/users/{userid}/objects:
    get:
      summary: Returns the list of monitoring items for the given userid
      description: Returns the list of monitoring items for the given userid.
      operationId: monitorSubforUserId
      x-api-path-slug: monitoringusersuseridobjects-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: offset
        description: Offset
      - in: query
        name: projectid
        description: Project Id
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Monitoring
      - Itemsthe
      - Given
      - Userid
  /monitoring/users/myself/objects/{objectid}:
    get:
      summary: The logged in user is monitoring the current object or not (true /
        false)
      description: The logged in user is monitoring the current object or not (true
        / false).
      operationId: isObjectMonitored
      x-api-path-slug: monitoringusersmyselfobjectsobjectid-get
      parameters:
      - in: path
        name: objectid
        description: Object id
      responses:
        200:
          description: OK
      tags:
      - The
      - Logged
      - In
      - User
      - Is
      - Monitoring
      - Current
      - Object
      - Not
      - (true
      - ""
      - ""
      - False)
  /monitoring/users/myself/objects:
    get:
      summary: Returns the list of monitoring items for current user
      description: Returns the list of monitoring items for current user.
      operationId: monitoringItemsForUser
      x-api-path-slug: monitoringusersmyselfobjects-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: offset
        description: Offset
      - in: query
        name: projectid
        description: Project id
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Monitoring
      - Itemscurrent
      - User
  /monitoring/users/by-username/{username}/objects/{objectid}:
    get:
      summary: Monitoring the current object or not for the given username (true /
        false)
      description: Monitoring the current object or not for the given username (true
        / false).
      operationId: isObjectMonitoredByUsername
      x-api-path-slug: monitoringusersbyusernameusernameobjectsobjectid-get
      parameters:
      - in: path
        name: objectid
        description: Object id
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Current
      - Object
      - Notthe
      - Given
      - Username
      - (true
      - ""
      - ""
      - False)
  /monitoring/users/by-username/{username}/objects:
    get:
      summary: Returns the list of monitoring items for the given username
      description: Returns the list of monitoring items for the given username.
      operationId: monitoringItemsForUsername
      x-api-path-slug: monitoringusersbyusernameusernameobjects-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: offset
        description: Offset
      - in: query
        name: projectid
        description: Project Id
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Monitoring
      - Itemsthe
      - Given
      - Username
  /monitoring/objects/{objectid}/users:
    get:
      summary: Returns the list of monitoring users for the object(Folder/Item).
      description: Returns the list of monitoring users for the object(folder/item)..
      operationId: listUsersForObject
      x-api-path-slug: monitoringobjectsobjectidusers-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: path
        name: objectid
        description: Object id
      - in: query
        name: offset
        description: Offset
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Monitoring
      - Usersthe
      - Object(Folder
      - Item)
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