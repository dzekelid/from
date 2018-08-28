swagger: "2.0"
x-collection-name: Docsmore
x-complete: 1
info:
  title: Docsmore API 2.1
  description: alt-texthttpswww-docsmore-comwpcontentuploads201802docsmoreapi-png-titleh3create-a-developer-account-at-docsmore-io-and-start-unleashing-the-power-of-docsmore-into-your-own-applications--to-make-it-easier-we-have-provided-client-libraries-and-sdk-in-several-languages-for-you-to-get-started-and-hit-the-ground-running-in-no-time-h3brbrh4note-if-you-dont-see-api-setting-under-top-right-menu-that-means-you-will-need-to-be-a-developer-account--please-contact-supportdocsmore-com-and-a-customer-service-expert-will-switch-your-account-to-developer-account--h4brbrh5just-head-over-to-httpsdocsmore-io-and-sign-up-for-your-30-days-trial-h5
  version: "1.0"
host: api.docsmore.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/getworkflowlink:
    post:
      summary: Get Workflow Link
      description: |-
        This is the most popular use of Docsmore API. From your connected app, you can launch workflow and obtain the unique link for immediate launch or later on. You can also supply data in flat json format that can be used inside the document for pre-fill purpose saving your customer time.

        Please make sure you pay close attention to the requirement for this API call as there are several aspects of it as required parameters.
      operationId: ApiGetworkflowlinkPost
      x-api-path-slug: apigetworkflowlink-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Link
  /api/dmcatalogue:
    post:
      summary: Fetch All Documents from Your Team Catalogue
      description: By design, the authenticated user can only view the files that
        are either created by them or shared with them. Make sure user has at least
        read permission to view the catalogue.
      operationId: ApiDmcataloguePost
      x-api-path-slug: apidmcatalogue-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: items
      - in: query
        name: page
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - ""
      - Documents
      - From
      - Your
      - Team
      - Catalogue