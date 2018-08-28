---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Get Alerts Events. Format
  version: 1.0.0
  description: "This API endpoint allows you to list the alert events for your account.\n\nAlerts
    events can be filter by product, target type, group ID, instance ID, and event
    type.\n\nThe options for products are: APM, BROWSER, MOBILE, SERVERS, PLUGINS,
    SYNTHETICS, and ALERTS.\n\nThe options for entity type are: Application, Server,
    KeyTransaction, Plugin, MobileApplication, BrowserApplication, and Monitor.\n\nThe
    options for event type are: NOTIFICATION, DEPLOYMENT, VIOLATION_OPEN, VIOLATION_CLOSE,
    VIOLATION, and INSTRUMENTATION.\n\nThe group ID option is normally the same as
    the entity ID (e.g. an Application group ID and entity ID will be the same), however
    PLUGINS have a group ID representing the PLUGIN itself, and entity IDs for all
    instances of that PLUGIN type.\n\nSee our documentation for a discussion on \noutput
    pagination."
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /alerts_events.{format}:
    get:
      summary: Get Alerts Events. Format
      description: "This API endpoint allows you to list the alert events for your
        account.\n\nAlerts events can be filter by product, target type, group ID,
        instance ID, and event type.\n\nThe options for products are: APM, BROWSER,
        MOBILE, SERVERS, PLUGINS, SYNTHETICS, and ALERTS.\n\nThe options for entity
        type are: Application, Server, KeyTransaction, Plugin, MobileApplication,
        BrowserApplication, and Monitor.\n\nThe options for event type are: NOTIFICATION,
        DEPLOYMENT, VIOLATION_OPEN, VIOLATION_CLOSE, VIOLATION, and INSTRUMENTATION.\n\nThe
        group ID option is normally the same as the entity ID (e.g. an Application
        group ID and entity ID will be the same), however PLUGINS have a group ID
        representing the PLUGIN itself, and entity IDs for all instances of that PLUGIN
        type.\n\nSee our documentation for a discussion on \noutput pagination."
      operationId: getAlertsEvents.Format
      x-api-path-slug: alerts-events-format-get
      parameters:
      - in: query
        name: filter[entity_group_id]
        description: Filter by entity group ID
        type: integer
      - in: query
        name: filter[entity_id]
        description: Filter by entity ID
        type: integer
      - in: query
        name: filter[entity_type]
        description: Filter by entity type
        type: string
      - in: query
        name: filter[event_type]
        description: Filter by event type
        type: string
      - in: query
        name: filter[product]
        description: Filter by New Relic product
        type: string
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Events.
      - Format
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