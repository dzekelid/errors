swagger: "2.0"
x-collection-name: Google Stackdriver Monitoring
x-complete: 1
info:
  title: Google Stackdriver Monitoring
  description: google-stackdriver-provides-powerful-monitoring-logging-and-diagnostics--it-equips-you-with-insight-into-the-health-performance-and-availability-of-cloudpowered-applications-enabling-you-to-find-and-fix-issues-faster--it-is-natively-integrated-with-google-cloud-platform-amazon-web-services-and-popular-open-source-packages--stackdriver-provides-a-wide-variety-of-metrics-dashboards-alerting-log-management-reporting-and-tracing-capabilities-
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
    get:
      summary: Get Project Name Events
      description: Lists the specified events.
      operationId: clouderrorreporting.projects.events.list
      x-api-path-slug: v1beta1projectnameevents-get
      parameters:
      - in: query
        name: groupId
        description: '[Required] The group for which events shall be returned'
      - in: query
        name: pageSize
        description: '[Optional] The maximum number of results to return per response'
      - in: query
        name: pageToken
        description: '[Optional] A `next_page_token` provided by a previous response'
      - in: path
        name: projectName
        description: '[Required] The resource name of the Google Cloud Platform project'
      - in: query
        name: serviceFilter.service
        description: '[Optional] The exact value to match against[`ServiceContext'
      - in: query
        name: serviceFilter.version
        description: '[Optional] The exact value to match against[`ServiceContext'
      - in: query
        name: timeRange.period
        description: Restricts the query to the specified time range
      responses:
        200:
          description: OK
      tags:
      - Errors
  /v1beta1/{projectName}/events:report:
    post:
      summary: Post Project Name Events Report
      description: Report an individual error event. This endpoint accepts <strong>either</strong>
        an OAuth token, or an API key for authentication. To use an API key, append
        it to the URL as the value of a `key` parameter.
      operationId: clouderrorreporting.projects.events.report
      x-api-path-slug: v1beta1projectnameeventsreport-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectName
        description: '[Required] The resource name of the Google Cloud Platform project'
      responses:
        200:
          description: OK
      tags:
      - Errors
  /v1beta1/{projectName}/groupStats:
    get:
      summary: Get Project Name Groupstats
      description: Lists the specified groups.
      operationId: clouderrorreporting.projects.groupStats.list
      x-api-path-slug: v1beta1projectnamegroupstats-get
      parameters:
      - in: query
        name: alignment
        description: '[Optional] The alignment of the timed counts to be returned'
      - in: query
        name: alignmentTime
        description: '[Optional] Time where the timed counts shall be aligned if roundedalignment
          is chosen'
      - in: query
        name: groupId
        description: '[Optional] List all ErrorGroupStats with these IDs'
      - in: query
        name: order
        description: '[Optional] The sort order in which the results are returned'
      - in: query
        name: pageSize
        description: '[Optional] The maximum number of results to return per response'
      - in: query
        name: pageToken
        description: '[Optional] A `next_page_token` provided by a previous response'
      - in: path
        name: projectName
        description: '[Required] The resource name of the Google Cloud Platform project'
      - in: query
        name: serviceFilter.service
        description: '[Optional] The exact value to match against[`ServiceContext'
      - in: query
        name: serviceFilter.version
        description: '[Optional] The exact value to match against[`ServiceContext'
      - in: query
        name: timedCountDuration
        description: '[Optional] The preferred duration for a single returned `TimedCount`'
      - in: query
        name: timeRange.period
        description: Restricts the query to the specified time range
      responses:
        200:
          description: OK
      tags:
      - Errors