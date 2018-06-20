---
swagger: "2.0"
x-collection-name: Alpha Vantage
x-complete: 0
info:
  title: Alpha Vantage Currency Exchange Rates
  description: Realtime currency exchange rates for physical and digital currencies.
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