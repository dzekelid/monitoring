swagger: "2.0"
x-collection-name: RingCentral
x-complete: 1
info:
  title: RingCentral Connect Platform API Explorer
  description: this-is-an-interactive-api-explorer-for-the-ringcentral-connect-platform--to-use-this-service-you-will-need-to-have-a-developer-account---links--a-hrefhttpsnetstorage-ringcentral-comdpwapiexplorerrcplatform-basic-ymlv20180514092722-target-blankringcentral-api-specaspannbspnbspopenapi-fka-swagger-formatnbspnbspnbspnbspspana-hrefhttpsgithub-comoaiopenapispecification-target-blanklearn-more-about-openapia
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/account/{accountId}/call-monitoring-groups:
    get:
      summary: Get Call Monitoring Groups
      description: |-
        Returns call monitoring groups that can be filtered by some extension.
        App Permission
        ReadAccounts
        User Permission
        ReadExtensions
        Usage Plan Group
        Medium
      operationId: listCallMonitoringGroups
      x-api-path-slug: restapiv1-0accountaccountidcallmonitoringgroups-get
      parameters:
      - in: path
        name: accountId
      - in: query
        name: memberExtensionId
        description: Internal identifier of an extension that is a member of every
          group within the result
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      responses:
        200:
          description: OK
      tags:
      - Call
      - Monitoring
      - Groups
  /restapi/v1.0/account/{accountId}/call-monitoring-groups/{groupId}/members:
    get:
      summary: Get Call Monitoring Group Members
      description: |-
        Returns call monitoring group members.
        App Permission
        ReadAccounts
        User Permission
        ReadExtensions
        Usage Plan Group
        Medium
      operationId: listCallMonitoringGroupMembers
      x-api-path-slug: restapiv1-0accountaccountidcallmonitoringgroupsgroupidmembers-get
      parameters:
      - in: path
        name: accountId
      - in: path
        name: groupId
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      responses:
        200:
          description: OK
      tags:
      - Call
      - Monitoring
      - Group
      - Members