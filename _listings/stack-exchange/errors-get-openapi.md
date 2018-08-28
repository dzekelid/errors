---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 0
info:
  title: Stack Exchange Get Errors
  description: "Returns the various error codes that can be produced by the API.\n
    \nThis method is provided for discovery, documentation, and testing purposes,
    it is not expected many applications will consume it during normal operation.\n
    \nFor testing purposes, look into the /errors/{id} method which simulates errors
    given a code.\n \nThis method returns a list of errors."
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /errors:
    get:
      summary: Get Errors
      description: "Returns the various error codes that can be produced by the API.\n
        \nThis method is provided for discovery, documentation, and testing purposes,
        it is not expected many applications will consume it during normal operation.\n
        \nFor testing purposes, look into the /errors/{id} method which simulates
        errors given a code.\n \nThis method returns a list of errors."
      operationId: returns-the-various-error-codes-that-can-be-produced-by-the-api-this-method-is-provided-for-discover
      x-api-path-slug: errors-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
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