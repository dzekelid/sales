---
swagger: "2.0"
x-collection-name: 3dcart
x-complete: 0
info:
  title: 3dcart Adds a new upselling item to the system
  version: 1.0.0
  description: Adds a new upselling item to the system.
host: apirest.3dcart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dCartWebAPI/v1/Products/{catalogid}/UpSelling:
    get:
      summary: Get the upselling products from a specific Product
      description: Get the upselling products from a specific product.
      operationId: Products_GetAllProductUpSelling
      x-api-path-slug: 3dcartwebapiv1productscatalogidupselling-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Upselling
      - Products
      - From
      - Specific
      - Product
    put:
      summary: Updates a collection of upselling items from a specific Product
      description: Updates a collection of upselling items from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidupselling-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: body
        name: upsellingitems
        description: A Json or XML object containing the new upselling items
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Upselling
      - Items
      - From
      - Specific
      - Product
    post:
      summary: Adds a new upselling item to the system
      description: Adds a new upselling item to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogidupselling-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: body
        name: upsellingitem
        description: A Json or XML object containing the new upselling item
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Upselling
      - Item
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/UpSelling/{upsellingindexid}:
    put:
      summary: Updates a specific Upselling Item from a specific Product
      description: Updates a specific upselling item from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidupsellingupsellingindexid-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: path
        name: upsellingindexid
        description: UpSellingIndexID
      - in: body
        name: upsellingitem
        description: A Json or XML object containing the new upselling tem
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Upselling
      - Item
      - From
      - Specific
      - Product
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