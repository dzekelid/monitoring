swagger: "2.0"
x-collection-name: CollabNet
x-complete: 1
info:
  title: Foundation API
  version: 1.0.0
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
    post:
      summary: Monitors / Unmonitors the list of objects for the given userid.
      description: Monitors / unmonitors the list of objects for the given userid..
      operationId: monitorOrUnmonitorObjectsByUserid
      x-api-path-slug: monitoringusersuseridobjects-post
      parameters:
      - in: query
        name: action
        description: To perform action
      - in: body
        name: body
        description: Monitor / Unmonitor items
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - Monitors
      - ""
      - ""
      - Unmonitors
      - List
      - Of
      - Objectsthe
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
    post:
      summary: Monitors the current object for current user.
      description: Monitors the current object for current user..
      operationId: monitorObjectForUser
      x-api-path-slug: monitoringusersmyselfobjectsobjectid-post
      parameters:
      - in: path
        name: objectid
        description: Object id
      responses:
        200:
          description: OK
      tags:
      - Monitors
      - Current
      - Objectcurrent
      - User
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
    post:
      summary: Monitors / Unmonitors the list of objects for current user.
      description: Monitors / unmonitors the list of objects for current user..
      operationId: monitorOrUnmonitorObjectsForUser
      x-api-path-slug: monitoringusersmyselfobjects-post
      parameters:
      - in: query
        name: action
        description: To perform action
      - in: body
        name: body
        description: Monitor / Unmonitor items
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitors
      - ""
      - ""
      - Unmonitors
      - List
      - Of
      - Objectscurrent
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
    post:
      summary: Monitors the current object for the given username.
      description: Monitors the current object for the given username..
      operationId: monitorObjectByUsername
      x-api-path-slug: monitoringusersbyusernameusernameobjectsobjectid-post
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
      - Monitors
      - Current
      - Objectthe
      - Given
      - Username
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
    post:
      summary: Monitors / Unmonitors the list of objects for the given username
      description: Monitors / unmonitors the list of objects for the given username.
      operationId: monitorOrUnmonitorObjectsByUsername
      x-api-path-slug: monitoringusersbyusernameusernameobjects-post
      parameters:
      - in: query
        name: action
        description: To perform action
      - in: body
        name: body
        description: Monitor / Unmonitor items
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Monitors
      - ""
      - ""
      - Unmonitors
      - List
      - Of
      - Objectsthe
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