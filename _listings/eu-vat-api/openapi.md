swagger: "2.0"
x-collection-name: EU VAT API
x-complete: 1
info:
  title: VAT API
  description: a-developer-friendly-api-to-help-your-business-achieve-vat-compliance
  version: "1"
host: vatapi.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /country-code-check:
    get:
      summary: Retrieve a countries VAT rates by its 2 digit country code
      description: Retrieve a countries vat rates by its 2 digit country code.
      operationId: country_code_check
      x-api-path-slug: countrycodecheck-get
      parameters:
      - in: query
        name: code
        description: The 2 digit country code
      - in: header
        name: Response-Type
        description: The default response type is application/json if you would like
          to receive an XML response then set this to XML
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Countries
      - VAT
      - Rates
      - By
      - Its
      - "2"
      - Digit
      - Country
      - Code
  /ip-check:
    get:
      summary: Retrieve a countries VAT rates from an IP address
      description: Retrieve a countries vat rates from an ip address.
      operationId: ip_check
      x-api-path-slug: ipcheck-get
      parameters:
      - in: query
        name: address
        description: The IP address to search against
      - in: header
        name: Response-Type
        description: The default response type is application/json if you would like
          to receive an XML response then set this to XML
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Countries
      - VAT
      - Rates
      - From
      - IP
      - Address
  /vat-rates:
    get:
      summary: Retrieve all current EU VAT rates
      description: Retrieve all current eu vat rates.
      operationId: vat_rates
      x-api-path-slug: vatrates-get
      parameters:
      - in: header
        name: Response-Type
        description: The default response type is application/json if you would like
          to receive an XML response then set this to XML
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - ""
      - Current
      - EU
      - VAT
      - Rates