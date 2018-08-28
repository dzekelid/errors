swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/admin/parser/log/error:
    post:
      summary: Post Admin Parser Log Error
      description: Post admin parser log error.
      operationId: postApiV1AdminParserLogError
      x-api-path-slug: apiv1adminparserlogerror-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Parser
      - Log
      - Error