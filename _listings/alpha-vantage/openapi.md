---
swagger: "2.0"
x-collection-name: Alpha Vantage
x-complete: 1
info:
  title: Alpha Vantage
  description: alpha-vantage-apis-are-grouped-into-four-categories-1-stock-time-series-data-2-physical-and-digitalcrypto-currencies-e-g--bitcoin-3-stock-technical-indicators-and-4-sector-performances--all-apis-are-realtime-the-latest-data-points-are-derived-from-the-current-trading-day--
  version: 1.0.0
host: www.alphavantage.co
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /query?function=CURRENCY_EXCHANGE_RATE:
    get:
      summary: Currency Exchange Rates
      description: Realtime currency exchange rates for physical and digital currencies.
      operationId: getCurrencyExchangeRates
      x-api-path-slug: queryfunctioncurrency-exchange-rate-get
      parameters:
      - in: query
        name: from_currency
        description: The currency you would like to get the exchange rate for
        type: string
        format: string
      - in: query
        name: to_currency
        description: The destination currency for the exchange rate
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Currency
      - Exchange Rates
---