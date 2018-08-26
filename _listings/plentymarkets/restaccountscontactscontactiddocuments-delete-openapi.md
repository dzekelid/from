---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Delete files from contact documents
  description: Delete files from contact documents.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounts/contacts/{contactId}/document:
    get:
      summary: Get a single storage object from contact documents
      description: Get a single storage object from contact documents.
      operationId: getRestAccountsContactsContactDocument
      x-api-path-slug: restaccountscontactscontactiddocument-get
      parameters:
      - in: path
        name: contactId
      - in: query
        name: key
        description: The storage key of the object to get from contact documents
      responses:
        200:
          description: OK
      tags:
      - Single
      - Storage
      - Object
      - From
      - Contact
      - Documents
  /rest/accounts/contacts/{contactId}/documents:
    delete:
      summary: Delete files from contact documents
      description: Delete files from contact documents.
      operationId: deleteRestAccountsContactsContactDocuments
      x-api-path-slug: restaccountscontactscontactiddocuments-delete
      parameters:
      - in: path
        name: contactId
      - in: query
        name: keyList
        description: List of storage keys to delete
      responses:
        200:
          description: OK
      tags:
      - Files
      - From
      - Contact
      - Documents
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