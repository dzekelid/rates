---
name: Ship Station
x-slug: ship-station
description: ShipStation is a web-based shipping solution that streamlines the order
  fulfillment process for your online business. ShipStation consolidates orders from
  over 70 ecommerce channels, creates shipping labels, packing slips, and pick lists
  in batch, communicates tracking information to your customers, provides endless
  automation, filters, and views, wireless printing, a mobile app, and a lot more.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Rates
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/rates/master/_listings/ship-station/apis.md
specificationVersion: "0.14"
apis:
- name: Ship Station Developer Portal - Get Rates
  x-api-slug: shipmentsgetrates-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/rates/master/_listings/ship-station/shipmentsgetrates-post-openapi.md
x-common:
- type: x-website
  url: http://bit.ly/_ShipStation
- type: x-api-gallery
  url: http://server.density.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ship.station.stack.network
- type: x-blog
  url: https://www.shipstation.com/blog/
- type: x-developer
  url: https://shipstation.docs.apiary.io/#
- type: x-github
  url: https://github.com/shipstation
- type: x-partners
  url: https://www.shipstation.com/partners/
- type: x-pricing
  url: https://www.shipstation.com/pricing/
- type: x-twitter
  url: https://twitter.com/ShipStation
- type: x-website
  url: http://shipstation.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---