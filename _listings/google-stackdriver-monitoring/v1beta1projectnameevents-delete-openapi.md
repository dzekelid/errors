---
swagger: "2.0"
x-collection-name: Google Stackdriver Monitoring
x-complete: 0
info:
  title: Google Stackdriver Monitoring Delete Project Name Events
  description: Deletes all error events of a given project.
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
  /v1beta1/{name}:
    put:
      summary: Put Name
      description: |-
        Replace the data for the specified group.
        Fails if the group does not exist.
      operationId: clouderrorreporting.projects.groups.update
      x-api-path-slug: v1beta1name-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The group resource name
      responses:
        200:
          description: OK
      tags:
      - Errors
  /v1beta1/{projectName}/events:
    delete:
      summary: Delete Project Name Events
      description: Deletes all error events of a given project.
      operationId: clouderrorreporting.projects.deleteEvents
      x-api-path-slug: v1beta1projectnameevents-delete
      parameters:
      - in: path
        name: projectName
        description: '[Required] The resource name of the Google Cloud Platform project'
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