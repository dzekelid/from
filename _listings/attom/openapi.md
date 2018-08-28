swagger: "2.0"
x-collection-name: ATTOM
x-complete: 1
info:
  title: Attom Data Solutions API
  description: attom-empowers-customers-with-better-property-data--we-warehouse-property-data-nationwide-with-myriad-data-points-on-each-parcel-including-ownership-information-latlong-square-footage-loan-types-sales-history-sales-comps-crime-schools-and-more-
  version: 1.0.0
host: search.onboard-apis.com
basePath: /communityapi/v2.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /school/snapshot:
    get:
      summary: Return all schools within a defined radius from a point.
      description: Search for all schools that are located within a given radius around
        a given latitude and longitude.
      operationId: propertySchoolSnapshot
      x-api-path-slug: schoolsnapshot-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: filetypetext
        description: The type of school (public, private, or catholic can be selected)
      - in: query
        name: latitude
        description: The property latitude coordinate
      - in: query
        name: longitude
        description: The property longitude coordinate
      - in: query
        name: radius
      responses:
        200:
          description: OK
      tags:
      - Return
      - ""
      - Schools
      - Within
      - Defined
      - Radius
      - From
      - Point