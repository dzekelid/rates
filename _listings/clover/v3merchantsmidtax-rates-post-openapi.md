---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Create a tax rate for a merchant
  version: 1.0.0
  description: Create a tax rate for a merchant.
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/tax_rates:
    get:
      summary: Get all tax rates
      description: Get all tax rates.
      operationId: GetTaxRates
      x-api-path-slug: v3merchantsmidtax-rates-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: query
        name: filter
        description: 'Filter fields: [isDefault, rate, items'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tax
      - Rates
    post:
      summary: Create a tax rate for a merchant
      description: Create a tax rate for a merchant.
      operationId: CreateTaxRate
      x-api-path-slug: v3merchantsmidtax-rates-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tax
      - Rates
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