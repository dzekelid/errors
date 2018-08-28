---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Utility APIs Create Error Report
  description: Create error report.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /error_reports:
    post:
      summary: Create Error Report
      description: Create error report.
      operationId: create-error-report
      x-api-path-slug: error-reports-post
      parameters:
      - in: query
        name: error[comments]
        description: The long version of the story from the user one what they experienced
      - in: query
        name: error[email]
        description: Email address for the reporting user
      - in: query
        name: error[http_env]
        description: A collection of metadata about the users&#39; environment
      - in: query
        name: error[subject]
        description: The summary of the problem
      - in: query
        name: error[url]
        description: URL from which the report was issued
      responses:
        200:
          description: OK
      tags:
      - Error
      - Reports
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