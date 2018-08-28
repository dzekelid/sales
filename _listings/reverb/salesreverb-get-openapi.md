---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 0
info:
  title: Reverb Get Sales Reverb
  description: View upcoming and live Reverb official sales.
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /listings/{listing_id}/sales:
    get:
      summary: Get Listings Listing Sales
      description: See all sales that include a listing.
      operationId: getListingsListingSales
      x-api-path-slug: listingslisting-idsales-get
      parameters:
      - in: path
        name: listing_id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Listing
      - Id
      - Sales
  /sales/reverb:
    get:
      summary: Get Sales Reverb
      description: View upcoming and live Reverb official sales.
      operationId: getSalesReverb
      x-api-path-slug: salesreverb-get
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Reverb
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