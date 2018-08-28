---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Rates Get WSJ Rate
  description: Returns a specific interest rate.
  version: 1.0.0
host: www.xignite.com
basePath: xRates.json/XigniteRates
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ListOfficialRates:
    get:
      summary: List Official Rates
      description: List supported official rates.
      operationId: postListofficialrates
      x-api-path-slug: listofficialrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Official
      - Rates
  /GetLatestCrossRates:
    get:
      summary: Get Latest Cross Rates
      description: Returns the latest possible cross rate.
      operationId: postGetlatestcrossrates
      x-api-path-slug: getlatestcrossrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Latest
      - Cross
      - Rates
  /GetRawCrossRates:
    get:
      summary: Get Raw Cross Rates
      description: Returns a real-time currency cross-rate.
      operationId: postGetrawcrossrates
      x-api-path-slug: getrawcrossrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Raw
      - Cross
      - Rates
  /GetRealTimeCrossRates:
    get:
      summary: Get Real Time Cross Rates
      description: Returns the latest possible cross rate.
      operationId: postGetrealtimecrossrates
      x-api-path-slug: getrealtimecrossrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Real
      - Time
      - Cross
      - Rates
  /GetAllCrossRatesForACurrency:
    get:
      summary: Get All Cross Rates For A Currency
      description: Returns all valid cross rates for a currency.
      operationId: postGetallcrossratesforacurrency
      x-api-path-slug: getallcrossratesforacurrency-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Cross
      - Rates
      - Currency
  /GetHistoricalCrossRates:
    get:
      summary: Get Historical Cross Rates
      description: Returns multiple cross-rates as of a historical date.
      operationId: postGethistoricalcrossrates
      x-api-path-slug: gethistoricalcrossrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rates
  /GetHistoricalCrossRatesBidAsk:
    get:
      summary: Get Historical Cross Rates Bid Ask
      description: Returns multiple cross-rates with bid/ask as of a historical date.
      operationId: postGethistoricalcrossratesbask
      x-api-path-slug: gethistoricalcrossratesbidask-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rates
      - Bid
      - Ask
  /GetHistoricalCrossRatesRange:
    get:
      summary: Get Historical Cross Rates Range
      description: This operation returns a range of cross-rates for a currency pair.
      operationId: postGethistoricalcrossratesrange
      x-api-path-slug: gethistoricalcrossratesrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rates
      - Range
  /GetHistoricalCrossRatesBidAskRange:
    get:
      summary: Get Historical Cross Rates Bid Ask Range
      description: This operation returns a range of cross-rates for a currency pair.
      operationId: postGethistoricalcrossratesbaskrange
      x-api-path-slug: gethistoricalcrossratesbidaskrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rates
      - Bid
      - Ask
      - Range
  /GetHistoricalCrossRatesAsOf:
    get:
      summary: Get Historical Cross Rates As Of
      description: This operation returns a range of cross-rates for a currency pair.
      operationId: postGethistoricalcrossratesasof
      x-api-path-slug: gethistoricalcrossratesasof-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rates
      - As
      - Of
  /GetHistoricalCrossRatesBidAskAsOf:
    get:
      summary: Get Historical Cross Rates Bid Ask As Of
      description: This operation returns a range of cross-rates for a currency pair.
      operationId: postGethistoricalcrossratesbaskasof
      x-api-path-slug: gethistoricalcrossratesbidaskasof-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rates
      - Bid
      - Ask
      - As
      - Of
  /GetOfficialCrossRates:
    get:
      summary: Get Official Cross Rates
      description: Returns an official cross-rate as of a historical date.
      operationId: postGetofficialcrossrates
      x-api-path-slug: getofficialcrossrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Official
      - Cross
      - Rates
  /GetOfficialCrossRatesBidAsk:
    get:
      summary: Get Official Cross Rates Bid Ask
      description: Returns an official cross-rate as of a historical date.
      operationId: postGetofficialcrossratesbask
      x-api-path-slug: getofficialcrossratesbidask-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Official
      - Cross
      - Rates
      - Bid
      - Ask
  /GetMutipleHistoricalCrossRates:
    get:
      summary: Get Mutiple Historical Cross Rates
      description: Returns multiple cross-rates as of a historical date.
      operationId: postGetmutiplehistoricalcrossrates
      x-api-path-slug: getmutiplehistoricalcrossrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Mutiple
      - Historical
      - Cross
      - Rates
  /GetAverageHistoricalCrossRates:
    get:
      summary: Get Average Historical Cross Rates
      description: This operation returns an array average daily historical cross-rates
        for a period.
      operationId: postGetaveragehistoricalcrossrates
      x-api-path-slug: getaveragehistoricalcrossrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Average
      - Historical
      - Cross
      - Rates
  /GetHistoricalMonthlyCrossRatesRange:
    get:
      summary: Get Historical Monthly Cross Rates Range
      description: This operation returns a complete range of stock quotes for a currency
        pair.
      operationId: postGethistoricalmonthlycrossratesrange
      x-api-path-slug: gethistoricalmonthlycrossratesrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Monthly
      - Cross
      - Rates
      - Range
  /GetRealTimeForwardRate:
    get:
      summary: Get Real Time Forward Rate
      description: Returns a set of real-time currency forward rates.
      operationId: postGetrealtimeforwardrate
      x-api-path-slug: getrealtimeforwardrate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Real
      - Time
      - Forward
      - Rate
  /GetRealTimeCrossRateAsString:
    get:
      summary: Get Real Time Cross Rate As String
      description: Returns a real-time currency cross-rate.
      operationId: postGetrealtimecrossrateasstring
      x-api-path-slug: getrealtimecrossrateasstring-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Real
      - Time
      - Cross
      - Rate
      - As
      - String
  /GetLatestCrossRate:
    get:
      summary: Get Latest Cross Rate
      description: Returns the latest possible cross rate.
      operationId: postGetlatestcrossrate
      x-api-path-slug: getlatestcrossrate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Latest
      - Cross
      - Rate
  /GetRealTimeCrossRate:
    get:
      summary: Get Real Time Cross Rate
      description: Returns a real-time currency cross-rate.
      operationId: postGetrealtimecrossrate
      x-api-path-slug: getrealtimecrossrate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Real
      - Time
      - Cross
      - Rate
  /GetRealTimeCrossRateGMT:
    get:
      summary: Get Real Time Cross Rate G M T
      description: Returns a real-time currency cross-rate with the times in GMT.
      operationId: postGetrealtimecrossrategmt
      x-api-path-slug: getrealtimecrossrategmt-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Real
      - Time
      - Cross
      - Rate
      - G
      - M
      - T
  /GetRawCrossRate:
    get:
      summary: Get Raw Cross Rate
      description: Returns a real-time currency cross-rate.
      operationId: postGetrawcrossrate
      x-api-path-slug: getrawcrossrate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Raw
      - Cross
      - Rate
  /GetHistoricalCrossRateTables:
    get:
      summary: Get Historical Cross Rate Tables
      description: Returns historical currency cross-rate tables for a range of dates.
      operationId: postGethistoricalcrossratetables
      x-api-path-slug: gethistoricalcrossratetables-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rate
      - Tables
  /GetHistoricalCrossRateTablesBidAsk:
    get:
      summary: Get Historical Cross Rate Tables Bid Ask
      description: Returns historical currency cross-rate tables for a range of dates.
      operationId: postGethistoricalcrossratetablesbask
      x-api-path-slug: gethistoricalcrossratetablesbidask-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rate
      - Tables
      - Bid
      - Ask
  /GetHistoricalCrossRateTable:
    get:
      summary: Get Historical Cross Rate Table
      description: Returns a historical currency cross-rate table.
      operationId: postGethistoricalcrossratetable
      x-api-path-slug: gethistoricalcrossratetable-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rate
      - Table
  /GetHistoricalCrossRateTableBidAsk:
    get:
      summary: Get Historical Cross Rate Table Bid Ask
      description: Returns a historical currency cross-rate table.
      operationId: postGethistoricalcrossratetablebask
      x-api-path-slug: gethistoricalcrossratetablebidask-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rate
      - Table
      - Bid
      - Ask
  /GetRealTimeCrossRateTable:
    get:
      summary: Get Real Time Cross Rate Table
      description: Returns a real-time currency cross-rate table.
      operationId: postGetrealtimecrossratetable
      x-api-path-slug: getrealtimecrossratetable-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Real
      - Time
      - Cross
      - Rate
      - Table
  /GetRealTimeCrossRateTableWithBidAsk:
    get:
      summary: Get Real Time Cross Rate Table With Bid Ask
      description: Returns a real-time currency cross-rate table.
      operationId: postGetrealtimecrossratetablewithbask
      x-api-path-slug: getrealtimecrossratetablewithbidask-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Real
      - Time
      - Cross
      - Rate
      - Table
      - With
      - Bid
      - Ask
  /GetRealTimeCrossRateTableAsHTML:
    get:
      summary: Get Real Time Cross Rate Table As H T M L
      description: Returns a real-time currency cross-rate table as an HTML Output.
      operationId: postGetrealtimecrossratetableashtml
      x-api-path-slug: getrealtimecrossratetableashtml-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Real
      - Time
      - Cross
      - Rate
      - Table
      - As
      - H
      - T
      - M
      - L
  /GetSimpleRealTimeCrossRateTableAsHTML:
    get:
      summary: Get Simple Real Time Cross Rate Table As H T M L
      description: Returns a real-time currency cross-rate table as an HTML Output.
      operationId: postGetsimplerealtimecrossratetableashtml
      x-api-path-slug: getsimplerealtimecrossratetableashtml-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Simple
      - Real
      - Time
      - Cross
      - Rate
      - Table
      - As
      - H
      - T
      - M
      - L
  /GetHistoricalCrossRateTableAsHTML:
    get:
      summary: Get Historical Cross Rate Table As H T M L
      description: Returns a historical currency cross-rate table as an HTML Output.
      operationId: postGethistoricalcrossratetableashtml
      x-api-path-slug: gethistoricalcrossratetableashtml-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rate
      - Table
      - As
      - H
      - T
      - M
      - L
  /GetHistoricalCrossRate:
    get:
      summary: Get Historical Cross Rate
      description: Returns a cross-rate as of a historical date.
      operationId: postGethistoricalcrossrate
      x-api-path-slug: gethistoricalcrossrate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rate
  /GetHistoricalCrossRateBidAsk:
    get:
      summary: Get Historical Cross Rate Bid Ask
      description: Returns a cross-rate with bid/ask as of a historical date.
      operationId: postGethistoricalcrossratebask
      x-api-path-slug: gethistoricalcrossratebidask-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rate
      - Bid
      - Ask
  /GetOfficialCrossRate:
    get:
      summary: Get Official Cross Rate
      description: Returns an official cross-rate as of a historical date.
      operationId: postGetofficialcrossrate
      x-api-path-slug: getofficialcrossrate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Official
      - Cross
      - Rate
  /GetOfficialCrossRateBidAsk:
    get:
      summary: Get Official Cross Rate Bid Ask
      description: Returns an official cross-rate as of a historical date.
      operationId: postGetofficialcrossratebask
      x-api-path-slug: getofficialcrossratebidask-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Official
      - Cross
      - Rate
      - Bid
      - Ask
  /GetAverageHistoricalCrossRate:
    get:
      summary: Get Average Historical Cross Rate
      description: This operation returns an average daily historical cross-rates
        for a period.
      operationId: postGetaveragehistoricalcrossrate
      x-api-path-slug: getaveragehistoricalcrossrate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Average
      - Historical
      - Cross
      - Rate
  /GetCrossRateChange:
    get:
      summary: Get Cross Rate Change
      description: This operation returns the changes in a cross-rates over the last
        6 months.
      operationId: postGetcrossratechange
      x-api-path-slug: getcrossratechange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Cross
      - Rate
      - Change
  /ListRates:
    get:
      summary: List Rates
      description: List supported interest rates.
      operationId: postListrates
      x-api-path-slug: listrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Rates
  /SearchRates:
    get:
      summary: Search Rates
      description: Search rate names and description
      operationId: postSearchrates
      x-api-path-slug: searchrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Search
      - Rates
  /GetHistoricalRates:
    get:
      summary: Get Historical Rates
      description: Returns a rate for a range of dates.
      operationId: postGethistoricalrates
      x-api-path-slug: gethistoricalrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Rates
  /GetRate:
    get:
      summary: Get Rate
      description: Returns a rate as of a specific date.
      operationId: postGetrate
      x-api-path-slug: getrate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
  /GetRateFamilyTable:
    get:
      summary: Get Rate Family Table
      description: Returns a rate table for a rate family.
      operationId: postGetratefamilytable
      x-api-path-slug: getratefamilytable-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - Family
      - Table
  /GetRateFamily:
    get:
      summary: Get Rate Family
      description: Returns a collection of related rate as of a specific date
      operationId: postGetratefamily
      x-api-path-slug: getratefamily-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - Family
  /GetTodaysRate:
    get:
      summary: Get Todays Rate
      description: Returns end of day closing value for a rate
      operationId: postGettodaysrate
      x-api-path-slug: gettodaysrate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Todays
      - Rate
  /GetLatestRate:
    get:
      summary: Get Latest Rate
      description: Returns latest value for a rate.
      operationId: postGetlatestrate
      x-api-path-slug: getlatestrate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Latest
      - Rate
  /GetLatestRateFamily:
    get:
      summary: Get Latest Rate Family
      description: Returns latest values for a rate family.
      operationId: postGetlatestratefamily
      x-api-path-slug: getlatestratefamily-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Latest
      - Rate
      - Family
  /GetHistoricalRateFamily:
    get:
      summary: Get Historical Rate Family
      description: Returns a rate family and for a range of dates.
      operationId: postGethistoricalratefamily
      x-api-path-slug: gethistoricalratefamily-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Rate
      - Family
  /GetRateDescription:
    get:
      summary: Get Rate Description
      description: Returns a description for a rate.
      operationId: postGetratedescription
      x-api-path-slug: getratedescription-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - Description
  Draw, Rate, , Custom:
    get:
      summary: Draw Rate Chart Custom
      description: Draw a custom rate chart for a date range.
      operationId: postDrawratechartcustom
      x-api-path-slug: draw-rate--custom-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Draw
      - Rate
      - Chart
      - Custom
  'Draw, Rate, ':
    get:
      summary: Draw Rate Chart
      description: Draw a standard rate chart for a date range.
      operationId: postDrawratechart
      x-api-path-slug: draw-rate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Draw
      - Rate
      - Chart
  Draw, Rate, , Preset:
    get:
      summary: Draw Rate Chart Preset
      description: Draw a standard rate chart for a date range.
      operationId: postDrawratechartpreset
      x-api-path-slug: draw-rate--preset-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Draw
      - Rate
      - Chart
      - Preset
  /ListSwapRates:
    get:
      summary: List Swap Rates
      description: Returns swap rate currencies and tenors
      operationId: postListswaprates
      x-api-path-slug: listswaprates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Swap
      - Rates
  /GetSwapRate:
    get:
      summary: Get Swap Rate
      description: Returns a Swap rate
      operationId: postGetswaprate
      x-api-path-slug: getswaprate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Swap
      - Rate
  /GetForwardRateAgreement:
    get:
      summary: Get Forward Rate Agreement
      description: Returns a calculated Forward Rate Agreement as of a date
      operationId: postGetforwardrateagreement
      x-api-path-slug: getforwardrateagreement-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Forward
      - Rate
      - Agreement
  /GetSwapRateFamily:
    get:
      summary: Get Swap Rate Family
      description: Returns a Swap rate Family
      operationId: postGetswapratefamily
      x-api-path-slug: getswapratefamily-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Swap
      - Rate
      - Family
  /GetHistoricalSwapRate:
    get:
      summary: Get Historical Swap Rate
      description: Returns a Swap rate as of a historical date
      operationId: postGethistoricalswaprate
      x-api-path-slug: gethistoricalswaprate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Swap
      - Rate
  /GetHistoricalSwapRateRange:
    get:
      summary: Get Historical Swap Rate Range
      description: Returns a Swap rate as of a historical date
      operationId: postGethistoricalswapraterange
      x-api-path-slug: gethistoricalswapraterange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Swap
      - Rate
      - Range
  /GetSwapRateExtended:
    get:
      summary: Get Swap Rate Extended
      description: Returns latest Swap rate
      operationId: postGetswaprateextended
      x-api-path-slug: getswaprateextended-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Swap
      - Rate
      - Extended
  /GetSwapRateFamilyExtended:
    get:
      summary: Get Swap Rate Family Extended
      description: Returns latest Swap rate family
      operationId: postGetswapratefamilyextended
      x-api-path-slug: getswapratefamilyextended-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Swap
      - Rate
      - Family
      - Extended
  /GetHistoricalSwapRateExtended:
    get:
      summary: Get Historical Swap Rate Extended
      description: Returns historical swap rate
      operationId: postGethistoricalswaprateextended
      x-api-path-slug: gethistoricalswaprateextended-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Swap
      - Rate
      - Extended
  /GetHistoricalSwapRateExtendedRange:
    get:
      summary: Get Historical Swap Rate Extended Range
      description: Returns historical Swap rate range
      operationId: postGethistoricalswaprateextendedrange
      x-api-path-slug: gethistoricalswaprateextendedrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Swap
      - Rate
      - Extended
      - Range
  /GetTreasuryRate:
    get:
      summary: Get Treasury Rate
      description: Returns a real-time Treasury rate
      operationId: postGettreasuryrate
      x-api-path-slug: gettreasuryrate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Treasury
      - Rate
  /GetTreasuryRateFamily:
    get:
      summary: Get Treasury Rate Family
      description: Returns a real-time Treasury rate family.
      operationId: postGettreasuryratefamily
      x-api-path-slug: gettreasuryratefamily-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Treasury
      - Rate
      - Family
  /GetStateRates:
    get:
      summary: Get State Rates
      description: Returns state rates for a date range.
      operationId: postGetstaterates
      x-api-path-slug: getstaterates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - State
      - Rates
  /GetFederalRates:
    get:
      summary: Get Federal Rates
      description: Returns federal discount borrowing for a date range.
      operationId: postGetfederalrates
      x-api-path-slug: getfederalrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Federal
      - Rates
  /ListRatesByRateFamily:
    get:
      summary: List Rates By Rate Family
      description: List supported interest rates from a RateFamilyType.
      operationId: postListratesbyratefamily
      x-api-path-slug: listratesbyratefamily-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Rates
      - Rate
      - Family
  /GetAverageRates:
    get:
      summary: Get Average Rates
      description: Returns average rate for a period.
      operationId: postGetaveragerates
      x-api-path-slug: getaveragerates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Average
      - Rates
  /GetHistoricalWeeklyRates:
    get:
      summary: Get Historical Weekly Rates
      description: Returns a rate for a range of dates.
      operationId: postGethistoricalweeklyrates
      x-api-path-slug: gethistoricalweeklyrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Weekly
      - Rates
  /GetFHLBankRates:
    get:
      summary: Get FHL Bank Rates
      description: Returns Federal Home Loan Bank rates.
      operationId: postGetfhlbankrates
      x-api-path-slug: getfhlbankrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - FHL
      - Bank
      - Rates
  /GetStateRate:
    get:
      summary: Get State Rate
      description: Returns a state rate
      operationId: postGetstaterate
      x-api-path-slug: getstaterate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - State
      - Rate
  /GetFederalRate:
    get:
      summary: Get Federal Rate
      description: Returns a federal discount borrowing rate
      operationId: postGetfederalrate
      x-api-path-slug: getfederalrate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Federal
      - Rate
  /GetWSJRate:
    get:
      summary: Get WSJ Rate
      description: Returns a specific interest rate.
      operationId: postGetwsjrate
      x-api-path-slug: getwsjrate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - WSJ
      - Rate
  /GetRateSymbol:
    get:
      summary: Get Rate Symbol
      description: Returns the symbol for a rate.
      operationId: postGetratesymbol
      x-api-path-slug: getratesymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - Symbol
  /GetRateFromSymbol:
    get:
      summary: Get Rate From Symbol
      description: Returns the symbol for a rate.
      operationId: postGetratefromsymbol
      x-api-path-slug: getratefromsymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - From
      - Symbol
  /GetAverageRate:
    get:
      summary: Get Average Rate
      description: Returns an average rate as of a specific date.
      operationId: postGetaveragerate
      x-api-path-slug: getaveragerate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Average
      - Rate
  /GetRateMovingAverage:
    get:
      summary: Get Rate Moving Average
      description: Returns a moving  average rate as of a specific date
      operationId: postGetratemovingaverage
      x-api-path-slug: getratemovingaverage-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - Moving
      - Average
  /GetLatestRateSpecial:
    get:
      summary: Get Latest Rate Special
      description: Returns latest value for a rate.
      operationId: postGetlatestratespecial
      x-api-path-slug: getlatestratespecial-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Latest
      - Rate
      - Special
  /GetRealTimeRate:
    get:
      summary: Get Real Time Rate
      description: Returns the value for a rate as of a specific time in the day.
      operationId: postGetrealtimerate
      x-api-path-slug: getrealtimerate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Real
      - Time
      - Rate
  /GetRateAsOfTime:
    get:
      summary: Get Rate As Of Time
      description: Returns the value for a rate as of a specific time in the day.
      operationId: postGetrateasoftime
      x-api-path-slug: getrateasoftime-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - As
      - Time
  /GetRateStatistics:
    get:
      summary: Get Rate Statistics
      description: Returns statistics for available rates.
      operationId: postGetratestatistics
      x-api-path-slug: getratestatistics-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - Statistics
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