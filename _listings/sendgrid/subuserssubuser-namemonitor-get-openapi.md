---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get Subusers Subuser Name Monitor
  description: Subuser monitor settings allow you to receive a sample of an outgoing
    message by a specific customer at a specific frequency of emails.
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subusers/{subuser_name}/monitor:
    delete:
      summary: Delete Subusers Subuser Name Monitor
      description: Subuser monitor settings allow you to receive a sample of an outgoing
        message by a specific customer at a specific frequency of emails.
      operationId: subusers.subuser_name.monitor.delete
      x-api-path-slug: subuserssubuser-namemonitor-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Subusers
      - Subuser
      - Name
      - Monitor
    get:
      summary: Get Subusers Subuser Name Monitor
      description: Subuser monitor settings allow you to receive a sample of an outgoing
        message by a specific customer at a specific frequency of emails.
      operationId: subusers.subuser_name.monitor.get
      x-api-path-slug: subuserssubuser-namemonitor-get
      responses:
        200:
          description: OK
      tags:
      - Email
      - Subusers
      - Subuser
      - Name
      - Monitor
    post:
      summary: Add Subusers Subuser Name Monitor
      description: Subuser monitor settings allow you to receive a sample of an outgoing
        message by a specific customer at a specific frequency of emails.
      operationId: subusers.subuser_name.monitor.post
      x-api-path-slug: subuserssubuser-namemonitor-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Subusers
      - Subuser
      - Name
      - Monitor
    put:
      summary: Put Subusers Subuser Name Monitor
      description: Subuser monitor settings allow you to receive a sample of an outgoing
        message by a specific customer at a specific frequency of emails.
      operationId: subusers.subuser_name.monitor.put
      x-api-path-slug: subuserssubuser-namemonitor-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Subusers
      - Subuser
      - Name
      - Monitor
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