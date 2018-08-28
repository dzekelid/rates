swagger: "2.0"
x-collection-name: nFusion Solutions
x-complete: 1
info:
  title: nFusion Solutions Market Data API v1
  description: nfusion-solutions-provides-rest-and-streaming-apis-that-deliver-enterprisegrade-financial-data--data-sets-include-realtime-and-historical-pricing-for-spot-prices-of-precious-metals-such-as-gold-silver-platinum-and-palladium-exchange-rates-for-major-currency-pairs-exchange-rates-for-crypto-currencies-such-as-btc-eth-and-ltc--all-api-access-requires-authentication--in-order-to-be-issued-access-credentials-you-must-first-enter-into-a-service-agreement-with-nfusion-solutions-and-acquire-a-commercial-license--for-information-on-how-to-obtain-a-licence-contact-salesnfusionsolutions-com-
  contact:
    name: nFusion Solutions
    url: https://nfusionsolutions.com/contact
    email: support@nfusionsolutions.com
  version: 1.0.0
host: api.nfusionsolutions.biz
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v{version}/Currencies/rate/supported:
    get:
      summary: Get list of currencies supported by the rate endpoint
      description: "Any of the currencies in this list can be paired with any other
        currency in this list when supplied to the Rate endpoint.\r\nFor example:
        USD/CAD,CAD/USD,USD/EUR,EUR/CAD"
      operationId: ApiV{versionCurrenciesRateSupportedGet
      x-api-path-slug: apivversioncurrenciesratesupported-get
      parameters:
      - in: query
        name: format
        description: to override content negotiation specify a value of json or xml
      - in: query
        name: token
        description: auth token
      - in: path
        name: version
        description: The requested API version
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Currencies
      - Supported
      - By
      - Rate
      - Endpoint