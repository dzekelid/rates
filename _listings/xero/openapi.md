---
swagger: "2.0"
x-collection-name: Xero
x-complete: 1
info:
  title: Accounting
  description: -introductionthe-xero-accounting-api-is-a-restful-web-service-and-uses-the-oauth-v1-0a-protocol-to-authenticate-3rd-party-applications--the-accounting-api-exposes-accounting-and-related-functions-of-the-main-xero-application-and-can-be-used-for-a-variety-of-purposes-such-as-creating-transactions-like-invoices-and-credit-notes-right-through-to-extracting-accounting-data-via-our-reports-endpoint-
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /TaxRates:
    get:
      summary: Get Taxrates
      description: Get taxrates.
      operationId: getTaxrates
      x-api-path-slug: taxrates-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - TaxRates
    post:
      summary: Post Taxrates
      description: Post taxrates.
      operationId: postTaxrates
      x-api-path-slug: taxrates-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: TaxRates
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - TaxRates
    put:
      summary: Put Taxrates
      description: Put taxrates.
      operationId: putTaxrates
      x-api-path-slug: taxrates-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: TaxRates
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - TaxRates
    x-related-model:
      summary: X-related-model Taxrates
      description: X-related-model taxrates.
      operationId: x-related-modelTaxrates
      x-api-path-slug: taxrates-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - TaxRates
---