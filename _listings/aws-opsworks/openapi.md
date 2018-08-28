swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 1
info:
  title: AWS OpsWorks API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeServiceErrors:
    get:
      summary: Describe Service Errors
      description: Describes AWS OpsWorks Stacks service errors.
      operationId: describeServiceErrors
      x-api-path-slug: actiondescribeserviceerrors-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      - in: query
        name: ServiceErrorIds
        description: An array of service error IDs
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Service
      - Errors