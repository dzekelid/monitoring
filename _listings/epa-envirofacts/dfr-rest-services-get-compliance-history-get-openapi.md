---
swagger: "2.0"
x-collection-name: EPA Envirofacts
x-complete: 0
info:
  title: U.S. EPA Enforcement and Compliance History Online (ECHO) - Detailed Facility
    Report (DFR) Detailed Facility Report 5 Year Compliance Monitoring History Service
  description: This procedure obtains data for the Compliance Monitoring History (5
    years) in the Enforcement and Compliance Section of the Detailed Facility report.
  contact:
    name: US EPA, OECA Integration, Targeting and Access Branch
  version: 0.0.0
host: ofmpub.epa.gov
basePath: /echo
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /dfr_rest_services.get_compliance_history:
    get:
      summary: Detailed Facility Report 5 Year Compliance Monitoring History Service
      description: This procedure obtains data for the Compliance Monitoring History
        (5 years) in the Enforcement and Compliance Section of the Detailed Facility
        report.
      operationId: this-procedure-obtains-data-for-the-compliance-monitoring-history-5-years-in-the-enforcement-and-com
      x-api-path-slug: dfr-rest-services-get-compliance-history-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environment
      - Detailed
      - Facility
      - Report
      - "5"
      - Year
      - Compliance
      - Monitoring
      - History
      - Service
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