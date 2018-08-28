---
swagger: "2.0"
x-collection-name: Intuit
x-complete: 0
info:
  title: QuickBooks Online V3 API Get Reports Department Sales
  description: |-
    Report - Department Sales
    Method : GET
  version: 1.0.0
host: DefaultParameterValue
basePath: /v3/company/DefaultParameterValue
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /salesreceipt/181:
    get:
      summary: Get SaleS Receipt
      description: |-
        Create an salesreceipt object
        Method : POST
      operationId: getSalesreceipt181
      x-api-path-slug: salesreceipt181-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - SaleS
      - Receipt
  /salesreceipt:
    post:
      summary: Post Sales Receipt
      description: |-
        Create an salesreceipt object
        Method : POST
      operationId: postSalesreceipt
      x-api-path-slug: salesreceipt-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Sales
      - Receipt
  /reports/ItemSales:
    get:
      summary: Get Reports Item Sales
      description: |-
        Report - Item Sales
        Method : GET

        Docs - https://developer.intuit.com/docs/api/accounting/sales%20by%20product
      operationId: getReportsItemsales
      x-api-path-slug: reportsitemsales-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Item
      - Sales
  /reports/DepartmentSales:
    get:
      summary: Get Reports Department Sales
      description: |-
        Report - Department Sales
        Method : GET
      operationId: getReportsDepartmentsales
      x-api-path-slug: reportsdepartmentsales-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Department
      - Sales
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