swagger: "2.0"
x-collection-name: Watchful
x-complete: 1
info:
  title: Watchful
  description: watchful-resulted-from-the-need-for-a-single-unified-dashboard-to-easily-monitor-all-of-the-web-sites-in-our-portfolios--after-years-of-evolution-our-solution-has-matured-into-a-simple-complete-and-professional-service--
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