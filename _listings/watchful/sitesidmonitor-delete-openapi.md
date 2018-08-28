---
swagger: "2.0"
x-collection-name: Watchful
x-complete: 0
info:
  title: Watchful Delete Uptime Monitor
  description: Return boolean
  version: 1.0.0
host: watchful.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /sites/{id}/monitor:
    delete:
      summary: Delete Uptime Monitor
      description: Return boolean
      operationId: deleteMonitor
      x-api-path-slug: sitesidmonitor-delete
      parameters:
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Monitor
    post:
      summary: Post Uptime Monitor
      description: Return boolean
      operationId: postMonitor
      x-api-path-slug: sitesidmonitor-post
      parameters:
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
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