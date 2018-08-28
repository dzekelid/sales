swagger: "2.0"
x-collection-name: Salesforce
x-complete: 1
info:
  title: Salesforce Sandbox
  description: create-sandbox-copies-of-your-environments-for-development-testing-and-training-without-compromising-the-data-and-applications-in-your-production-environment-
  version: 1.0.0
host: na14.salesforce.com
basePath: /services/data/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:
    get:
      summary: Get
      description: Lists summary information about each Salesforce version currently
        available, including the version, label, and a link to each version's root.
      operationId: get
      x-api-path-slug: get
      responses:
        200:
          description: OK
      tags:
      - ""