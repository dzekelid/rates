---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Get API All Asset Pair Rates
  version: 1.0.0
  description: Get api all asset pair rates.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/AllAssetPairRates:
    get:
      summary: Get API All Asset Pair Rates
      description: Get api all asset pair rates.
      operationId: ApiAllAssetPairRatesGet
      x-api-path-slug: apiallassetpairrates-get
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Pair
      - Rates
  /api/AllAssetPairRates/{id}:
    get:
      summary: Get API All Asset Pair Rates
      description: Get api all asset pair rates.
      operationId: ApiAllAssetPairRatesByIdGet
      x-api-path-slug: apiallassetpairratesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Pair
      - Rates
  /api/AssetPairDetailedRates:
    get:
      summary: Get API Assetpairdetailedrates
      description: Get api assetpairdetailedrates.
      operationId: ApiAssetPairDetailedRatesGet
      x-api-path-slug: apiassetpairdetailedrates-get
      parameters:
      - in: query
        name: assetId
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: period
      - in: query
        name: points
      - in: query
        name: withBid
      responses:
        200:
          description: OK
      tags:
      - Assetpairdetailedrates
  /api/AssetPairRates:
    get:
      summary: Get API Assetpairrates
      description: Get api assetpairrates.
      operationId: ApiAssetPairRatesGet
      x-api-path-slug: apiassetpairrates-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: ignoreBase
      responses:
        200:
          description: OK
      tags:
      - Assetpairrates
  /api/AssetPairRates/{id}:
    get:
      summary: Get API Assetpairrates
      description: Get api assetpairrates.
      operationId: ApiAssetPairRatesByIdGet
      x-api-path-slug: apiassetpairratesid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Assetpairrates
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