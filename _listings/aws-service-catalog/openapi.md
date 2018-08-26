---
swagger: "2.0"
x-collection-name: AWS Service Catalog
x-complete: 1
info:
  title: AWS Service Catalog API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DisassociatePrincipalFromPortfolio:
    get:
      summary: Disassociate Principal From Portfolio
      description: |-
        Disassociates a previously associated principal ARN from a specified
                 portfolio.
      operationId: disassociatePrincipalFromPortfolio
      x-api-path-slug: actiondisassociateprincipalfromportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      - in: query
        name: PrincipalARN
        description: The ARN representing the principal (IAM user, role, or group)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=DisassociateProductFromPortfolio:
    get:
      summary: Disassociate Product From Portfolio
      description: Disassociates the specified product from the specified portfolio.
      operationId: disassociateProductFromPortfolio
      x-api-path-slug: actiondisassociateproductfromportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
---