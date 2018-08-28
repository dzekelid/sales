---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite NASDAQ Last Sale Get Last Sales By Identifiers
  description: Returns a real-time quote for a security based on the last trade execution.
  version: 1.0.0
host: nasdaqlastsale.xignite.com
basePath: xNASDAQLastSale.json/XigniteNASDAQLastSale
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetLastSales:
    get:
      summary: Get Last Sales
      description: Returns a collection of real time stock quotes for a comma-separated
        list of stock quotes.
      operationId: GetLastSales
      x-api-path-slug: getlastsales-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Last
      - Sales
  /GetLastSale:
    get:
      summary: Get Last Sale
      description: Returns Last Sale price for a specific bond as reported by the
        price source selected in the input. Request against this operation counts
        as one hit.
      operationId: GetLastSale
      x-api-path-slug: getlastsale-get
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
      - Last
      - Sale
  /GetLastSalesByIdentifiers:
    get:
      summary: Get Last Sales By Identifiers
      description: Returns a real-time quote for a security based on the last trade
        execution.
      operationId: GetLastSalesByIdentifiers
      x-api-path-slug: getlastsalesbyidentifiers-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Last
      - Sales
      - Identifiers
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