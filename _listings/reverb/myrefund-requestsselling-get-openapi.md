---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 0
info:
  title: Reverb Get My Refund Requests Selling
  description: Get a list of refund requests as a seller
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
  /listings/facets/seller_location:
    get:
      summary: Get Listings Facets Seller Location
      description: Get listings facets seller location.
      operationId: getListingsFacetsSellerLocation
      x-api-path-slug: listingsfacetsseller-location-get
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Facets
      - Seller
      - Location
  /orders/{order_id}/feedback/seller:
    get:
      summary: Get Orders Order Feedback Seller
      description: Feedback details for an order's seller
      operationId: getOrdersOrderFeedbackSeller
      x-api-path-slug: ordersorder-idfeedbackseller-get
      parameters:
      - in: path
        name: order_id
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Order
      - Id
      - Feedback
      - Seller
    post:
      summary: Post Orders Order Feedback Seller
      description: Add feedback about an order's seller
      operationId: postOrdersOrderFeedbackSeller
      x-api-path-slug: ordersorder-idfeedbackseller-post
      parameters:
      - in: path
        name: order_id
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Order
      - Id
      - Feedback
      - Seller
  /shops/{slug}/feedback/seller:
    get:
      summary: Get Shops Slug Feedback Seller
      description: Get seller's feedback as a seller
      operationId: getShopsSlugFeedbackSeller
      x-api-path-slug: shopsslugfeedbackseller-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Slug
      - Feedback
      - Seller
  /my/orders/buying/buying_history/{seller_id}:
    get:
      summary: Get My Orders Buying Buying History Seller
      description: Get my orders buying buying history seller.
      operationId: getMyOrdersBuyingBuyingHistorySeller
      x-api-path-slug: myordersbuyingbuying-historyseller-id-get
      parameters:
      - in: path
        name: seller_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Buying
      - Buying
      - History
      - Seller
      - Id
  /my/orders/selling/all:
    get:
      summary: Get My Orders Selling All
      description: Get all seller orders, newest first.
      operationId: getMyOrdersSellingAll
      x-api-path-slug: myorderssellingall-get
      parameters:
      - in: query
        name: created_end_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: created_start_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: updated_end_date
        description: Filter by date modified in ISO8601 format - e
      - in: query
        name: updated_start_date
        description: Filter by date modified in ISO8601 format - e
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
  /my/orders/selling/awaiting_shipment:
    get:
      summary: Get My Orders Selling Awaiting Shipment
      description: Get seller orders awaiting shipment, newest first.
      operationId: getMyOrdersSellingAwaitingShipment
      x-api-path-slug: myorderssellingawaiting-shipment-get
      parameters:
      - in: query
        name: created_end_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: created_start_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: updated_end_date
        description: Filter by date modified in ISO8601 format - e
      - in: query
        name: updated_start_date
        description: Filter by date modified in ISO8601 format - e
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Awaiting
      - Shipment
  /my/orders/selling/buyer_history/{buyer_id}:
    get:
      summary: Get My Orders Selling Buyer History Buyer
      description: Get my orders selling buyer history buyer.
      operationId: getMyOrdersSellingBuyerHistoryBuyer
      x-api-path-slug: myorderssellingbuyer-historybuyer-id-get
      parameters:
      - in: path
        name: buyer_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Buyer
      - History
      - Buyer
      - Id
  /my/orders/selling/unpaid:
    get:
      summary: Get My Orders Selling Unpa
      description: Get unpaid seller orders, newest first.
      operationId: getMyOrdersSellingUnpa
      x-api-path-slug: myorderssellingunpaid-get
      parameters:
      - in: query
        name: created_end_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: created_start_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: updated_end_date
        description: Filter by date modified in ISO8601 format - e
      - in: query
        name: updated_start_date
        description: Filter by date modified in ISO8601 format - e
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Unpaid
  /my/orders/selling/{id}:
    get:
      summary: Get My Orders Selling
      description: Returns order details for a seller
      operationId: getMyOrdersSelling
      x-api-path-slug: myorderssellingid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Id
  /my/orders/selling/{id}/mark_picked_up:
    post:
      summary: Post My Orders Selling Mark Picked Up
      description: Post my orders selling mark picked up.
      operationId: postMyOrdersSellingMarkPickedUp
      x-api-path-slug: myorderssellingidmark-picked-up-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Id
      - Mark
      - Picked
      - Up
  /my/orders/selling/{id}/ship:
    post:
      summary: Post My Orders Selling Ship
      description: Post my orders selling ship.
      operationId: postMyOrdersSellingShip
      x-api-path-slug: myorderssellingidship-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Id
      - Ship
  /my/orders/selling/{order_id}/refund_requests:
    post:
      summary: Post My Orders Selling Order Refund Requests
      description: Post my orders selling order refund requests.
      operationId: postMyOrdersSellingOrderRefundRequests
      x-api-path-slug: myorderssellingorder-idrefund-requests-post
      parameters:
      - in: path
        name: order_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Order
      - Id
      - Refund
      - Requests
  /my/payments/selling:
    get:
      summary: Get My Payments Selling
      description: Get my payments selling.
      operationId: getMyPaymentsSelling
      x-api-path-slug: mypaymentsselling-get
      parameters:
      - in: query
        name: created_end_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: created_start_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: offset
      - in: query
        name: order_id
        description: Look up payments by order id
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: updated_end_date
        description: Filter by date modified in ISO8601 format - e
      - in: query
        name: updated_start_date
        description: Filter by date modified in ISO8601 format - e
      responses:
        200:
          description: OK
      tags:
      - My
      - Payments
      - Selling
  /my/payments/selling/{id}:
    get:
      summary: Get My Payments Selling
      description: Get my payments selling.
      operationId: getMyPaymentsSelling
      x-api-path-slug: mypaymentssellingid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Payments
      - Selling
      - Id
  /my/refund_requests/selling:
    get:
      summary: Get My Refund Requests Selling
      description: Get a list of refund requests as a seller
      operationId: getMyRefundRequestsSelling
      x-api-path-slug: myrefund-requestsselling-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Refund
      - Requests
      - Selling
  /my/refund_requests/selling/{id}:
    put:
      summary: Put My Refund Requests Selling
      description: Update a refund request for a sold order
      operationId: putMyRefundRequestsSelling
      x-api-path-slug: myrefund-requestssellingid-put
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Refund
      - Requests
      - Selling
      - Id
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