swagger: "2.0"
x-collection-name: EU VAT API
x-complete: 1
info:
  title: VAT API
  description: a-developer-friendly-api-to-help-your-business-achieve-vat-compliance
  version: "1"
host: vatapi.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ip-check:
    get:
      summary: Retrieve a countries VAT rates from an IP address
      description: Retrieve a countries vat rates from an ip address.
      operationId: ip_check
      x-api-path-slug: ipcheck-get
      parameters:
      - in: query
        name: address
        description: The IP address to search against
      - in: header
        name: Response-Type
        description: The default response type is application/json if you would like
          to receive an XML response then set this to XML
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Countries
      - VAT
      - Rates
      - From
      - IP
      - Address
  /vat-price:
    get:
      summary: Convert a price to or from VAT price.
      description: Convert a price to or from vat price..
      operationId: convert_price
      x-api-path-slug: vatprice-get
      parameters:
      - in: query
        name: code
        description: The 2 digit country code
      - in: query
        name: country_rate
        description: The VAT rate to get the price for
      - in: query
        name: price
        description: The price you want converting
      - in: header
        name: Response-Type
        description: The default response type is application/json if you would like
          to receive an XML response then set this to XML
      - in: query
        name: type
        description: Optional, if the price is including VAT set the type to incl
      responses:
        200:
          description: OK
      tags:
      - Convert
      - Price
      - To
      - From
      - VAT
      - Price