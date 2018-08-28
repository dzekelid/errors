---
swagger: "2.0"
x-collection-name: Runscope
x-complete: 0
info:
  title: Runscope Get Buckets Errors
  description: Retrieve a list of error messages in a bucket
  version: 1.0.0
host: api.runscope.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /buckets/{bucketKey}/errors:
    get:
      summary: Get Buckets Errors
      description: Retrieve a list of error messages in a bucket
      operationId: buckets.bucketKey.errors.get
      x-api-path-slug: bucketsbucketkeyerrors-get
      parameters:
      - in: query
        name: before
        description: Only return messages before the given Unix timestamp
      - in: query
        name: count
        description: Maxiumum number of messages to return
      - in: query
        name: No Name
      - in: query
        name: since
        description: Only return messages after the given Unix timestamp
      responses:
        200:
          description: OK
      tags:
      - Buckets
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