swagger: "2.0"
x-collection-name: Google Search Console
x-complete: 1
info:
  title: Google Search Console URL Testing Tools
  description: provides-tools-for-running-validation-tests-against-single-urls
  contact:
    name: Google
    url: https://google.com
  version: v1
host: searchconsole.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /sites/{siteUrl}/urlCrawlErrorsCounts/query:
    get:
      summary: Get Crawl Error Count
      description: Retrieves a time series of the number of URL crawl errors per error
        category and platform.
      operationId: webmasters.urlcrawlerrorscounts.query
      x-api-path-slug: sitessiteurlurlcrawlerrorscountsquery-get
      parameters:
      - in: query
        name: category
        description: The crawl error category
      - in: query
        name: latestCountsOnly
        description: If true, returns only the latest crawl error counts
      - in: query
        name: platform
        description: The user agent type (platform) that made the request
      - in: path
        name: siteUrl
        description: The sites URL, including protocol
      responses:
        200:
          description: OK
      tags:
      - Error
  /sites/{siteUrl}/urlCrawlErrorsSamples:
    get:
      summary: Get Crawl Error Samples
      description: Lists a site's sample URLs for the specified crawl error category
        and platform.
      operationId: webmasters.urlcrawlerrorssamples.list
      x-api-path-slug: sitessiteurlurlcrawlerrorssamples-get
      parameters:
      - in: query
        name: category
        description: The crawl error category
      - in: query
        name: platform
        description: The user agent type (platform) that made the request
      - in: path
        name: siteUrl
        description: The sites URL, including protocol
      responses:
        200:
          description: OK
      tags:
      - Error
  /sites/{siteUrl}/urlCrawlErrorsSamples/{url}:
    delete:
      summary: Delete Crawl Error Samples
      description: Marks the provided site's sample URL as fixed, and removes it from
        the samples list.
      operationId: webmasters.urlcrawlerrorssamples.markAsFixed
      x-api-path-slug: sitessiteurlurlcrawlerrorssamplesurl-delete
      parameters:
      - in: query
        name: category
        description: The crawl error category
      - in: query
        name: platform
        description: The user agent type (platform) that made the request
      - in: path
        name: siteUrl
        description: The sites URL, including protocol
      - in: path
        name: url
        description: The relative path (without the site) of the sample URL
      responses:
        200:
          description: OK
      tags:
      - Error
    get:
      summary: Get Crawl Error Sample
      description: Retrieves details about crawl errors for a site's sample URL.
      operationId: webmasters.urlcrawlerrorssamples.get
      x-api-path-slug: sitessiteurlurlcrawlerrorssamplesurl-get
      parameters:
      - in: query
        name: category
        description: The crawl error category
      - in: query
        name: platform
        description: The user agent type (platform) that made the request
      - in: path
        name: siteUrl
        description: The sites URL, including protocol
      - in: path
        name: url
        description: The relative path (without the site) of the sample URL
      responses:
        200:
          description: OK
      tags:
      - Error