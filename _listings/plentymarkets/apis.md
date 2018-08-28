---
name: Plentymarkets
x-slug: plentymarkets
description: plentymarkets is an all-in-one e-commerce ERP solution, which combines
  a comprehensive stock management system with a versatile shop system and effortless
  multichannel sales. Thanks to comprehensive functions and interfaces that include
  all steps of the e-commerce value chain, you can use the cloud based software to
  completely automate all of your e-business processes as well as your companys own
  individual processes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
x-kinRank: "7"
x-alexaRank: ""
tags: Sales
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/apis.md
specificationVersion: "0.14"
apis:
- name: plentymarkets REST-API - List sales prices
  x-api-slug: restitemssales-prices-get
  description: Lists all sales prices.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemssales-prices-get-openapi.md
- name: plentymarkets REST-API - Create a sales price
  x-api-slug: restitemssales-prices-post
  description: Creates a sales price.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemssales-prices-post-openapi.md
- name: plentymarkets REST-API - Delete a sales price
  x-api-slug: restitemssales-pricesid-delete
  description: |-
    Deletes a sales price. The ID of the sales price must be specified.

    Delete salesPrice
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemssales-pricesid-delete-openapi.md
- name: plentymarkets REST-API - Get a sales price
  x-api-slug: restitemssales-pricesid-get
  description: Gets the data for a specific sales price. The ID of the sales price
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemssales-pricesid-get-openapi.md
- name: plentymarkets REST-API - Update a sales price
  x-api-slug: restitemssales-pricesid-put
  description: Updates a sales price.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemssales-pricesid-put-openapi.md
- name: plentymarkets REST-API - List countries by sales price
  x-api-slug: restitemssales-pricesidcountries-get
  description: Lists active countries for a sales price. The ID of the sales price
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemssales-pricesidcountries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemssales-pricesidcountries-get-openapi.md
- name: plentymarkets REST-API - List names of a sales price
  x-api-slug: restitemssales-pricesidnames-get
  description: Lists the names of a sales price in all languages. The ID of the sales
    price must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemssales-pricesidnames-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemssales-pricesidnames-get-openapi.md
- name: plentymarkets REST-API - Create a sales price name
  x-api-slug: restitemssales-pricesidnames-post
  description: Creates a name for a sales price in the specified language. The ID
    of the sales price must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemssales-pricesidnames-post-openapi.md
- name: plentymarkets REST-API - Delete a sales price name
  x-api-slug: restitemssales-pricesidnameslang-delete
  description: Deletes the name of a sales price in the specified language. The ID
    of the sales price and the language code must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemssales-pricesidnameslang-delete-openapi.md
- name: plentymarkets REST-API - Gets a sales price name
  x-api-slug: restitemssales-pricesidnameslang-get
  description: Gets the sales price name of a sales price in the specified langauge.
    The ID of the sales price and the language code must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemssales-pricesidnameslang-get-openapi.md
- name: plentymarkets REST-API - Update a sales price name
  x-api-slug: restitemssales-pricesidnameslang-put
  description: Updates a sales price name in the specified language. The ID of the
    sales price and the language code must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemssales-pricesidnameslang-put-openapi.md
- name: plentymarkets REST-API - Get all sales price relations
  x-api-slug: restitemsvariationsvariation-sales-prices-get
  description: Gets all links between variations and sales prices including sales
    price data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemsvariationsvariation-sales-prices-get-openapi.md
- name: plentymarkets REST-API - Delete all links between a variation and its sales
    prices
  x-api-slug: restitemsidvariationsvariationidvariation-sales-prices-delete
  description: Deletes all links between a variation and its sales prices and deletes
    the sales price data. The ID of the variation must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemsidvariationsvariationidvariation-sales-prices-delete-openapi.md
- name: plentymarkets REST-API - List sales prices of a variation
  x-api-slug: restitemsidvariationsvariationidvariation-sales-prices-get
  description: Lists the sales prices of a variation. The ID of the variation must
    be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemsidvariationsvariationidvariation-sales-prices-get-openapi.md
- name: plentymarkets REST-API - Create link between variation and sales price
  x-api-slug: restitemsidvariationsvariationidvariation-sales-prices-post
  description: Creates a link between a variation and a sales price and adds sales
    price data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemsidvariationsvariationidvariation-sales-prices-post-openapi.md
- name: plentymarkets REST-API - Delete link between variation and sales price
  x-api-slug: restitemsidvariationsvariationidvariation-sales-pricespriceid-delete
  description: Deletes a link between a variation and a sales price and deletes the
    sales price data. The ID of the sales price and the ID of the variation must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemsidvariationsvariationidvariation-sales-pricespriceid-delete-openapi.md
- name: plentymarkets REST-API - Get sales price data for a variation
  x-api-slug: restitemsidvariationsvariationidvariation-sales-pricespriceid-get
  description: Gets sales price data linked to a variation. The ID of the sales price
    and the ID of the variation must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemsidvariationsvariationidvariation-sales-pricespriceid-get-openapi.md
- name: plentymarkets REST-API - Update sales price data
  x-api-slug: restitemsidvariationsvariationidvariation-sales-pricespriceid-put
  description: Updates sales price data linked to a variation. The ID of the sales
    price and the ID of the variation must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/sales/master/_listings/plentymarkets/restitemsidvariationsvariationidvariation-sales-pricespriceid-put-openapi.md
x-common:
- type: x-blog-rss
  url: https://www.plentymarkets.co.uk/?ActionCall=WebActionRSS&rrss_id=1
- type: x-github
  url: https://github.com/plentymarkets
- type: x-twitter
  url: https://twitter.com/plentymarketsuk
- type: x-website
  url: http://www.plentymarkets.co.uk
- type: x-api-gallery
  url: http://pivotal.tracker.api.gallery.streamdata.io
- type: x-api-stack
  url: http://plentymarkets.stack.network
- type: x-blog
  url: https://www.plentymarkets.co.uk/blog/
- type: x-pricing
  url: https://www.plentymarkets.co.uk/prices/
- type: x-website
  url: https://www.plentymarkets.co.uk
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---