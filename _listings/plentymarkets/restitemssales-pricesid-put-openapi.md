---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Update a sales price
  description: Updates a sales price.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/items/sales_prices:
    get:
      summary: List sales prices
      description: Lists all sales prices.
      operationId: getRestItemsSalesPrices
      x-api-path-slug: restitemssales-prices-get
      parameters:
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      responses:
        200:
          description: OK
      tags:
      - List
      - Sales
      - Prices
    post:
      summary: Create a sales price
      description: Creates a sales price.
      operationId: postRestItemsSalesPrices
      x-api-path-slug: restitemssales-prices-post
      parameters:
      - in: body
        name: /rest/items/sales_prices
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Price
  /rest/items/sales_prices/{id}:
    delete:
      summary: Delete a sales price
      description: |-
        Deletes a sales price. The ID of the sales price must be specified.

        Delete salesPrice
      operationId: deleteRestItemsSalesPrices
      x-api-path-slug: restitemssales-pricesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Price
    get:
      summary: Get a sales price
      description: Gets the data for a specific sales price. The ID of the sales price
        must be specified.
      operationId: getRestItemsSalesPrices
      x-api-path-slug: restitemssales-pricesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Price
    put:
      summary: Update a sales price
      description: Updates a sales price.
      operationId: putRestItemsSalesPrices
      x-api-path-slug: restitemssales-pricesid-put
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Price
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