---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Rates Draw Rate Chart Custom
  description: Draw a custom rate chart for a date range.
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
  Currency, , Custom:
    get:
      summary: Get Currency Chart Custom
      description: Draw a custom currency chart for a date range.
      operationId: postGetcurrencychartcustom
      x-api-path-slug: currency--custom-get
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
      - Currency
      - Chart
      - Custom
  Currency, , Custom, Binary:
    get:
      summary: Get Currency Chart Custom Binary
      description: Draw a custom currency chart for a date range.
      operationId: postGetcurrencychartcustombinary
      x-api-path-slug: currency--custom-binary-get
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
      - Currency
      - Chart
      - Custom
      - Binary
  Currency, Intraday, , Custom, Binary:
    get:
      summary: Get Currency Intraday Chart Custom Binary
      description: Draw a intraday currency chart for a time range in a binary format
      operationId: postGetcurrencyintradaychartcustombinary
      x-api-path-slug: currency-intraday--custom-binary-get
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
      - Currency
      - Intraday
      - Chart
      - Custom
      - Binary
  Currency, Intraday, , Custom:
    get:
      summary: Get Currency Intraday Chart Custom
      description: Draw a intraday currency chart for a time range in a binary format
      operationId: postGetcurrencyintradaychartcustom
      x-api-path-slug: currency-intraday--custom-get
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
      - Currency
      - Intraday
      - Chart
      - Custom
  Intraday, Future, , Custom:
    get:
      summary: Get Intraday Future Chart Custom
      description: Get a custom intraday price chart for a future contract.
      operationId: postGetintradayfuturechartcustom
      x-api-path-slug: intraday-future--custom-get
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
      - Intraday
      - Future
      - Chart
      - Custom
  Intraday, Future, , Custom, Binary:
    get:
      summary: Get Intraday Future Chart Custom Binary
      description: Get a custom intraday price chart for a future contract in binary
        format.
      operationId: postGetintradayfuturechartcustombinary
      x-api-path-slug: intraday-future--custom-binary-get
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
      - Intraday
      - Future
      - Chart
      - Custom
      - Binary
  Historical, Future, , Custom:
    get:
      summary: Get Historical Future Chart Custom
      description: Get a custom historical chart for a future contract in binary format.
      operationId: postGethistoricalfuturechartcustom
      x-api-path-slug: historical-future--custom-get
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
      - Future
      - Chart
      - Custom
  Historical, Future, , Custom, Binary:
    get:
      summary: Get Historical Future Chart Custom Binary
      description: Draw a custom historical chart for a future contract.
      operationId: postGethistoricalfuturechartcustombinary
      x-api-path-slug: historical-future--custom-binary-get
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
      - Future
      - Chart
      - Custom
      - Binary
  Historical, Commodity, , Custom:
    get:
      summary: Get Historical Commodity Chart Custom
      description: Get a custom historical chart for a commodity in binary format.
      operationId: postGethistoricalcommoditychartcustom
      x-api-path-slug: historical-commodity--custom-get
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
      - Commodity
      - Chart
      - Custom
  Historical, Commodity, , Custom, Binary:
    get:
      summary: Get Historical Commodity Chart Custom Binary
      description: Draw a custom historical chart for a future contract.
      operationId: postGethistoricalcommoditychartcustombinary
      x-api-path-slug: historical-commodity--custom-binary-get
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
      - Commodity
      - Chart
      - Custom
      - Binary
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
  /DrawYieldCurveCustom:
    get:
      summary: Draw Yield Curve Custom
      description: Draw a yield curve for a rate family.
      operationId: postDrawyieldcurvecustom
      x-api-path-slug: drawyieldcurvecustom-get
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
      - Yield
      - Curve
      - Custom
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