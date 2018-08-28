swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Client/properties/isUserFromUS:
    get:
      summary: Get API Client Properties Isuserfromus
      description: Get api client properties isuserfromus.
      operationId: ApiClientPropertiesIsUserFromUSGet
      x-api-path-slug: apiclientpropertiesisuserfromus-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Client
      - Properties
      - Isuserfromus
    post:
      summary: Add API Client Properties Isuserfromus
      description: Add api client properties isuserfromus.
      operationId: ApiClientPropertiesIsUserFromUSPost
      x-api-path-slug: apiclientpropertiesisuserfromus-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Client
      - Properties
      - Isuserfromus