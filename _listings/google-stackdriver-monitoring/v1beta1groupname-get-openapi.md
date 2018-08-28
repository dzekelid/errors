---
swagger: "2.0"
x-collection-name: Google Stackdriver Monitoring
x-complete: 0
info:
  title: Google Stackdriver Monitoring Get Groupname
  description: Get the specified group.
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1beta1/{groupName}:
    get:
      summary: Get Groupname
      description: Get the specified group.
      operationId: ""
      x-api-path-slug: v1beta1groupname-get
      parameters:
      - in: path
        name: groupName
        description: '[Required] The group resource name'
      responses:
        200:
          description: OK
      tags:
      - Errors
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