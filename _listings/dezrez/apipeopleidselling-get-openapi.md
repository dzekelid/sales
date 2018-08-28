---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get Selling Roles for a Person
  version: 1.0.0
  description: Get selling roles for a person.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/todo/assignleadstopredefinedteams:
    put:
      summary: Assign InboundLead Todos to the predefined neg teams. e.g. Sales Valuers,
        Sales Viewings, Lettings Viewings etc etc
      description: Assign inboundlead todos to the predefined neg teams. e.g. sales
        valuers, sales viewings, lettings viewings etc etc.
      operationId: DefaultToDo_AssignLeadsToPredefinedTeamsBytoDoId
      x-api-path-slug: apitodoassignleadstopredefinedteams-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: toDoId
      responses:
        200:
          description: OK
      tags:
      - Assign
      - InboundLead
      - Todos
      - To
      - Predefined
      - Neg
      - Teams
      - ""
      - E
      - G
      - ""
      - Sales
      - Valuers
      - ""
      - Sales
      - Viewings
      - ""
      - Lettings
      - Viewings
      - Etc
      - Etc
  /api/documentgeneration/salesapplicantwelcomepack:
    post:
      summary: Generates a correspondence to a an sales applicant
      description: Generates a correspondence to a an sales applicant.
      operationId: DocumentGeneration_SalesApplicantWelcomePackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationsalesapplicantwelcomepack-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Sales
      - Applicant
  /api/group/{id}/salessearching:
    get:
      summary: Get Sales Searching Roles for a Group
      description: Get sales searching roles for a group.
      operationId: Group_SearchingSalesRolesByidBypageSizeBypageNumber
      x-api-path-slug: apigroupidsalessearching-get
      parameters:
      - in: path
        name: id
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Searching
      - Rolesa
      - Group
  /api/negotiator/my/properties/{roleType}:
    get:
      summary: Used for the Property Sales Dashboard to return a list of the negotiator's
        properties.
      description: Used for the property sales dashboard to return a list of the negotiator's
        properties..
      operationId: Negotiator_PropertiesByroleTypeBypageSizeBypageNumber
      x-api-path-slug: apinegotiatormypropertiesroletype-get
      parameters:
      - in: query
        name: pageNumber
        description: which page number of results to choose
      - in: query
        name: pageSize
        description: how many properties to return (default 10)
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleType
        description: the PropertyMarketingRole type
      responses:
        200:
          description: OK
      tags:
      - Usedthe
      - Property
      - Sales
      - Dashboard
      - To
      - Return
      - List
      - Of
      - Negotiators
      - Properties
  /api/progression/withdrawinstruction:
    put:
      summary: Add withdrawalvaluation to a property sales role
      description: Add withdrawalvaluation to a property sales role.
      operationId: Progression_WithdrawInstructionBywithdrawInstructionDataContract
      x-api-path-slug: apiprogressionwithdrawinstruction-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: withdrawInstructionDataContract
        description: Details of the progression withdrawal
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Withdrawalvaluation
      - To
      - Property
      - Sales
      - Role
  /api/progression/withdrawvaluation:
    put:
      summary: Add WithdrawVal to a property sales role
      description: Add withdrawval to a property sales role.
      operationId: Progression_WithdrawValuationBywithdrawValuationDataContract
      x-api-path-slug: apiprogressionwithdrawvaluation-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: withdrawValuationDataContract
        description: Details of the progression withdrawal
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - WithdrawVal
      - To
      - Property
      - Sales
      - Role
  /api/progressionchain/{id}/additem:
    post:
      summary: Add item to sales progression chain
      description: Add item to sales progression chain.
      operationId: ProgressionChain_AddItemToChainByidBydataContract
      x-api-path-slug: apiprogressionchainidadditem-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Progression Role Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Item
      - To
      - Sales
      - Progression
      - Chain
  /api/progressionchain/{id}/updateitem:
    put:
      summary: Update item in sales progression chain
      description: Update item in sales progression chain.
      operationId: ProgressionChain_UpdateChainItemByidBydataContract
      x-api-path-slug: apiprogressionchainidupdateitem-put
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Progression Role Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Item
      - In
      - Sales
      - Progression
      - Chain
  /api/progression/sales/exchange:
    post:
      summary: Exchanges a sales role
      description: Exchanges a sales role.
      operationId: SalesProgression_ExchangeByexchangeCommandDataContract
      x-api-path-slug: apiprogressionsalesexchange-post
      parameters:
      - in: body
        name: exchangeCommandDataContract
        description: Details of the exchange
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Exchanges
      - Sales
      - Role
  /api/progression/sales/complete:
    post:
      summary: Completes a sales role
      description: Completes a sales role.
      operationId: SalesProgression_CompleteBycompleteCommandDataContract
      x-api-path-slug: apiprogressionsalescomplete-post
      parameters:
      - in: body
        name: completeCommandDataContract
        description: Details of the completion
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Completes
      - Sales
      - Role
  /api/offer/recordoffer:
    post:
      summary: Record offer on a sale
      description: Record offer on a sale.
      operationId: Offer_RecordOfferByofferCommand
      x-api-path-slug: apiofferrecordoffer-post
      parameters:
      - in: body
        name: offerCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Offer
      - "On"
      - Sale
  /api/offer/recordofferresponse:
    post:
      summary: Record a sale/auction offer response
      description: Record a sale/auction offer response.
      operationId: Offer_RecordOfferResponseByrecordOfferResponseCommand
      x-api-path-slug: apiofferrecordofferresponse-post
      parameters:
      - in: body
        name: recordOfferResponseCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Sale
      - Auction
      - Offer
      - Response
  /api/people/{id}/selling:
    get:
      summary: Get Selling Roles for a Person
      description: Get selling roles for a person.
      operationId: People_SellingRolesByid
      x-api-path-slug: apipeopleidselling-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Selling
      - Rolesa
      - Person
  /api/role/{id}/updateprice:
    put:
      summary: Update price for a given PropertySalesRole.
      description: Update price for a given propertysalesrole..
      operationId: Role_UpdatePriceByidByupdatePriceDataContract
      x-api-path-slug: apiroleidupdateprice-put
      parameters:
      - in: path
        name: id
        description: the id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: updatePriceDataContract
        description: UpdatePriceDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Pricea
      - Given
      - PropertySalesRole
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