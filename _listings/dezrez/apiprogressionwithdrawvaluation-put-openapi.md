---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Add WithdrawVal to a property sales role
  version: 1.0.0
  description: Add withdrawval to a property sales role.
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