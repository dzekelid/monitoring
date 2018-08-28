---
swagger: "2.0"
x-collection-name: API Science
x-complete: 0
info:
  title: API Science Poll Monitor
  version: 1.0.0
  description: Poll a monitor.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /monitors:
    get:
      summary: Get All Monitors
      description: Marks message as read.
      operationId: getAllMonitors
      x-api-path-slug: monitors-get
      parameters:
      - in: header
        name: Authorization
        description: Your API key must be included in all API requests to the server
          in an Authorization HTTP header
      - in: query
        name: tags
        description: Optionally filter monitors by tags
      responses:
        200:
          description: OK
      tags:
      - Monitors
    post:
      summary: Create Monitor
      description: Create a new monitor.
      operationId: create-monitor
      x-api-path-slug: monitors-post
      responses:
        200:
          description: OK
      tags:
      - Monitors
    put:
      summary: Apply Actions to Multiple Monitors
      description: Apply Actions to Multiple Monitors
      operationId: applyActionsToMultipleMonitors
      x-api-path-slug: monitors-put
      parameters:
      - in: path
        name: tags
        description: Optionally filter monitors by tags
      responses:
        200:
          description: OK
      tags:
      - Monitors
  /monitors/{id}:
    get:
      summary: Get a Specific Monitor
      description: Get a Specific Monitor
      operationId: getMonitor
      x-api-path-slug: monitorsid-get
      parameters:
      - in: path
        name: id
        description: The ID of the monitor to retrieve
      responses:
        200:
          description: OK
      tags:
      - Monitors
  /monitors/{id}/test:
    get:
      summary: Testing your Monitor
      description: Testing your Monitor
      operationId: testMonitor
      x-api-path-slug: monitorsidtest-get
      responses:
        200:
          description: OK
      tags:
      - Monitors
  /monitors/{monitor_id}:
    put:
      summary: Update Monitor
      description: Update an existing monitor
      operationId: update-monitor
      x-api-path-slug: monitorsmonitor-id-put
      parameters:
      - in: path
        name: monitor_id
        description: MandatoryUnique ID of the monitor
        type: <td>string</td>
      responses:
        200:
          description: OK
      tags:
      - Monitors
  /monitors/activate/{monitor_id}:
    put:
      summary: Activate Monitor
      description: Activate a suspended monitor
      operationId: activate-monitor
      x-api-path-slug: monitorsactivatemonitor-id-put
      parameters:
      - in: path
        name: monitor_id
        description: MandatoryUnique ID of the monitor
        type: <td>string</td>
      responses:
        200:
          description: OK
      tags:
      - Monitors
  /monitor/poll_now/{monitor_id}:
    get:
      summary: Poll Monitor
      description: Poll a monitor.
      operationId: poll-monitor
      x-api-path-slug: monitorpoll-nowmonitor-id-get
      parameters:
      - in: path
        name: monitor_id
        description: MandatoryUnique ID of the monitor
        type: <td>string</td>
      responses:
        200:
          description: OK
      tags:
      - Monitors
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