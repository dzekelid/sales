---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 0
info:
  title: Reverb Get Sales Slug
  description: Get sales slug.
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
  /sales/seller:
    get:
      summary: Get Sales Seller
      description: View your created sales.
      operationId: getSalesSeller
      x-api-path-slug: salesseller-get
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Seller
  /sales/{sale_id}/listings:
    delete:
      summary: Delete Sales Sale Listings
      description: Remove a listing from a sale
      operationId: deleteSalesSaleListings
      x-api-path-slug: salessale-idlistings-delete
      parameters:
      - in: path
        name: sale_id
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Sale
      - Id
      - Listings
    post:
      summary: Post Sales Sale Listings
      description: Post sales sale listings.
      operationId: postSalesSaleListings
      x-api-path-slug: salessale-idlistings-post
      parameters:
      - in: path
        name: sale_id
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Sale
      - Id
      - Listings
  /sales/{slug}:
    get:
      summary: Get Sales Slug
      description: Get sales slug.
      operationId: getSalesSlug
      x-api-path-slug: salesslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Slug
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