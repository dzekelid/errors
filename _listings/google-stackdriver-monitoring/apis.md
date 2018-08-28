---
name: Google Stackdriver Monitoring
x-slug: google-stackdriver-monitoring
description: Google Stackdriver provides powerful monitoring, logging, and diagnostics.
  It equips you with insight into the health, performance, and availability of cloud-powered
  applications, enabling you to find and fix issues faster. It is natively integrated
  with Google Cloud Platform, Amazon Web Services, and popular open source packages.
  Stackdriver provides a wide variety of metrics, dashboards, alerting, log management,
  reporting, and tracing capabilities.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-stackdriver.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Errors
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/errors/master/_listings/google-stackdriver-monitoring/apis.md
specificationVersion: "0.14"
apis:
- name: Google Stackdriver Monitoring - Get Groupname
  x-api-slug: v1beta1groupname-get
  description: Get the specified group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-stackdriver.png
  humanURL: https://cloud.google.com/monitoring/docs/
  baseURL: https:///
  tags: Monitoring, Stack Network, API Service Provider, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/errors/master/_listings/google-stackdriver-monitoring/v1beta1groupname-get-openapi.md
- name: Google Stackdriver Monitoring - Put Name
  x-api-slug: v1beta1name-put
  description: |-
    Replace the data for the specified group.
    Fails if the group does not exist.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-stackdriver.png
  humanURL: https://cloud.google.com/monitoring/docs/
  baseURL: https:///
  tags: Monitoring, Stack Network, API Service Provider, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/errors/master/_listings/google-stackdriver-monitoring/v1beta1name-put-openapi.md
- name: Google Stackdriver Monitoring - Delete Project Name Events
  x-api-slug: v1beta1projectnameevents-delete
  description: Deletes all error events of a given project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-stackdriver.png
  humanURL: https://cloud.google.com/monitoring/docs/
  baseURL: https:///
  tags: Monitoring, Stack Network, API Service Provider, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/errors/master/_listings/google-stackdriver-monitoring/v1beta1projectnameevents-delete-openapi.md
- name: Google Stackdriver Monitoring - Get Project Name Events
  x-api-slug: v1beta1projectnameevents-get
  description: Lists the specified events.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-stackdriver.png
  humanURL: https://cloud.google.com/monitoring/docs/
  baseURL: https:///
  tags: Monitoring, Stack Network, API Service Provider, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/errors/master/_listings/google-stackdriver-monitoring/v1beta1projectnameevents-get-openapi.md
- name: Google Stackdriver Monitoring - Post Project Name Events Report
  x-api-slug: v1beta1projectnameeventsreport-post
  description: Report an individual error event. This endpoint accepts <strong>either</strong>
    an OAuth token, or an API key for authentication. To use an API key, append it
    to the URL as the value of a `key` parameter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-stackdriver.png
  humanURL: https://cloud.google.com/monitoring/docs/
  baseURL: https:///
  tags: Monitoring, Stack Network, API Service Provider, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/errors/master/_listings/google-stackdriver-monitoring/v1beta1projectnameeventsreport-post-openapi.md
- name: Google Stackdriver Monitoring - Get Project Name Groupstats
  x-api-slug: v1beta1projectnamegroupstats-get
  description: Lists the specified groups.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-stackdriver.png
  humanURL: https://cloud.google.com/monitoring/docs/
  baseURL: https:///
  tags: Monitoring, Stack Network, API Service Provider, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/errors/master/_listings/google-stackdriver-monitoring/v1beta1projectnamegroupstats-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.speech.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.stackdriver.monitoring.stack.network
- type: x-developer
  url: https://cloud.google.com/monitoring/api/v3/
- type: x-website
  url: https://cloud.google.com/monitoring/docs/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---