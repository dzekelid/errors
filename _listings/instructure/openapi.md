swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Utility APIs
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
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