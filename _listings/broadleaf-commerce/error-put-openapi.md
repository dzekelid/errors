---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 0
info:
  title: Broadleaf Commerce API Put Error
  description: Put error.
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /error:
    get:
      summary: Get Error
      description: Get error.
      operationId: getError
      x-api-path-slug: error-get
      responses:
        200:
          description: OK
      tags:
      - Error
    head:
      summary: Head Error
      description: Head error.
      operationId: headError
      x-api-path-slug: error-head
      responses:
        200:
          description: OK
      tags:
      - Head
      - Error
    post:
      summary: Post Error
      description: Post error.
      operationId: postError
      x-api-path-slug: error-post
      responses:
        200:
          description: OK
      tags:
      - Error
    put:
      summary: Put Error
      description: Put error.
      operationId: putError
      x-api-path-slug: error-put
      responses:
        200:
          description: OK
      tags:
      - Error
    delete:
      summary: Delete Error
      description: Delete error.
      operationId: deleteError
      x-api-path-slug: error-delete
      responses:
        200:
          description: OK
      tags:
      - Error
    options:
      summary: Options Error
      description: Options error.
      operationId: optionsError
      x-api-path-slug: error-options
      responses:
        200:
          description: OK
      tags:
      - Options
      - Error
    patch:
      summary: Patch Error
      description: Patch error.
      operationId: patchError
      x-api-path-slug: error-patch
      responses:
        200:
          description: OK
      tags:
      - Error
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