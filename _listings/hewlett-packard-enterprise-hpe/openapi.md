swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 1
info:
  title: HPE OneSphere API
  description: hpe-onesphere-hybrid-cloud-management-rest-api-for-calls-requiring-authentication-use-restsession-to-get-a-token-
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rates:
    get:
      summary: Get Rates
      description: |-
        Returns rates. It requires the **administrator** global role.

        Optionally this list may be filtered, or the default rates specified with a resourceUri of 'default'.
      operationId: listRates
      x-api-path-slug: rates-get
      parameters:
      - in: query
        name: active
        description: Filter for active or inactive rates
      - in: query
        name: count
        description: Maximum number of response members to return
      - in: query
        name: effectiveDate
        description: The specific effective date to filter by
      - in: query
        name: effectiveForDate
        description: The date for which returned rates need be effective, a special
          filter that allows a search for a rate that would be effective on a date
      - in: query
        name: metricName
        description: The metric name to filter by
      - in: query
        name: resourceUri
        description: Resource(s) to return rates for
      - in: query
        name: start
        description: Index into the response members to allow pagination
      responses:
        200:
          description: OK
      tags:
      - Rates
  /rates/{id}:
    get:
      summary: Get Rates
      description: Retrieve a rate by id. It requires the **administrator** global
        role.
      operationId: getRateById
      x-api-path-slug: ratesid-get
      parameters:
      - in: path
        name: id
        description: Id of the rate to be retrieved
      responses:
        200:
          description: OK
      tags:
      - Rates