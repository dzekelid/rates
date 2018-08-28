---
swagger: "2.0"
x-collection-name: Ship Station
x-complete: 0
info:
  title: Ship Station Get Rates
  description: "Retrieves shipping rates for the specified shipping details.  The
    body of this request should specify the following attributes:\n\nName               |Data
    Type          |Description\n-------------------|-------------------|-------------------\n
    ``carrierCode`` | string, required | Returns rates for the specified carrier.\n
    ``serviceCode`` | string, optional | Returns rates for the specified shipping
    service.\n ``packageCode`` | string, optional | Returns rates for the specified
    package type.\n ``fromPostalCode`` | string, required | Originating postal code.\n
    ``toState`` | string, optional | Destination State/Province. Please use two-character
    state/province abbreviation. Note this field is required for the following carriers:
    UPS\n ``toCountry`` | string, required | Destination Country.  Please use the
    two-character ISO country code.\n ``toPostalCode`` | string, required | Destination
    Postal Code.\n ``toCity`` | string, optional | Destination City.\n ``weight``
    | Weight, required | Shipment's weight.  Use ``Weight`` object.\n ``dimensions``
    | Dimensions, optional | Shipment's dimensions.  Use ``Dimensions`` object. \n
    ``confirmation`` | string, optional | Returns rates that account for the specified
    delivery confirmation type.\n ``residential`` | boolean, optional | Returns rates
    that account for the specified delivery confirmation type. Default value: false"
  version: 1.0.0
host: ssapi.shipstation.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shipments/getrates:
    post:
      summary: Get Rates
      description: "Retrieves shipping rates for the specified shipping details.  The
        body of this request should specify the following attributes:\n\nName               |Data
        Type          |Description\n-------------------|-------------------|-------------------\n
        ``carrierCode`` | string, required | Returns rates for the specified carrier.\n
        ``serviceCode`` | string, optional | Returns rates for the specified shipping
        service.\n ``packageCode`` | string, optional | Returns rates for the specified
        package type.\n ``fromPostalCode`` | string, required | Originating postal
        code.\n ``toState`` | string, optional | Destination State/Province. Please
        use two-character state/province abbreviation. Note this field is required
        for the following carriers: UPS\n ``toCountry`` | string, required | Destination
        Country.  Please use the two-character ISO country code.\n ``toPostalCode``
        | string, required | Destination Postal Code.\n ``toCity`` | string, optional
        | Destination City.\n ``weight`` | Weight, required | Shipment's weight.  Use
        ``Weight`` object.\n ``dimensions`` | Dimensions, optional | Shipment's dimensions.
        \ Use ``Dimensions`` object. \n ``confirmation`` | string, optional | Returns
        rates that account for the specified delivery confirmation type.\n ``residential``
        | boolean, optional | Returns rates that account for the specified delivery
        confirmation type. Default value: false"
      operationId: shipments.getrates.post
      x-api-path-slug: shipmentsgetrates-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
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