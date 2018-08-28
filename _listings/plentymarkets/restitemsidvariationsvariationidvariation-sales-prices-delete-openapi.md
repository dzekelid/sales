---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Delete all links between a variation and its sales prices
  description: Deletes all links between a variation and its sales prices and deletes
    the sales price data. The ID of the variation must be specified.
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
  /rest/items/sales_prices/{id}/countries:
    get:
      summary: List countries by sales price
      description: Lists active countries for a sales price. The ID of the sales price
        must be specified.
      operationId: getRestItemsSalesPricesCountries
      x-api-path-slug: restitemssales-pricesidcountries-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Countries
      - By
      - Sales
      - Price
  /rest/items/sales_prices/{id}/names:
    get:
      summary: List names of a sales price
      description: Lists the names of a sales price in all languages. The ID of the
        sales price must be specified.
      operationId: getRestItemsSalesPricesNames
      x-api-path-slug: restitemssales-pricesidnames-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
      - Of
      - Sales
      - Price
    post:
      summary: Create a sales price name
      description: Creates a name for a sales price in the specified language. The
        ID of the sales price must be specified.
      operationId: postRestItemsSalesPricesNames
      x-api-path-slug: restitemssales-pricesidnames-post
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}/names
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
      - Name
  /rest/items/sales_prices/{id}/names/{lang}:
    delete:
      summary: Delete a sales price name
      description: Deletes the name of a sales price in the specified language. The
        ID of the sales price and the language code must be specified.
      operationId: deleteRestItemsSalesPricesNamesLang
      x-api-path-slug: restitemssales-pricesidnameslang-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Price
      - Name
    get:
      summary: Gets a sales price name
      description: Gets the sales price name of a sales price in the specified langauge.
        The ID of the sales price and the language code must be specified.
      operationId: getRestItemsSalesPricesNamesLang
      x-api-path-slug: restitemssales-pricesidnameslang-get
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - S
      - Sales
      - Price
      - Name
    put:
      summary: Update a sales price name
      description: Updates a sales price name in the specified language. The ID of
        the sales price and the language code must be specified.
      operationId: putRestItemsSalesPricesNamesLang
      x-api-path-slug: restitemssales-pricesidnameslang-put
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}/names/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Price
      - Name
  /rest/items/variations/variation_sales_prices:
    get:
      summary: Get all sales price relations
      description: Gets all links between variations and sales prices including sales
        price data.
      operationId: getRestItemsVariationsVariationSalesPrices
      x-api-path-slug: restitemsvariationsvariation-sales-prices-get
      parameters:
      - in: query
        name: salesPriceId
        description: Filter that restricts the search result to the sales price data
          of variations linked to a specific sales price
      - in: query
        name: updatedAt
        description: Filter that restricts the search result to links between variations
          and sales prices updated after a specific point in time
      - in: query
        name: variationId
        description: Filter that restricts the search result to the sales price data
          of a specific variation
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Price
      - Relations
  /rest/items/{id}/variations/{variationId}/variation_sales_prices:
    delete:
      summary: Delete all links between a variation and its sales prices
      description: Deletes all links between a variation and its sales prices and
        deletes the sales price data. The ID of the variation must be specified.
      operationId: deleteRestItemsVariationsVariationVariationSalesPrices
      x-api-path-slug: restitemsidvariationsvariationidvariation-sales-prices-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Links
      - Between
      - Variation
      - Its
      - Sales
      - Prices
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