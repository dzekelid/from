---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Unlink a client from a variation
  description: Deletes the link between a client (store) and a variation.
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
  /rest/accounts/contacts/{contactId}/vcard:
    get:
      summary: get a filestream of vcard from customer
      description: Get a filestream of vcard from customer.
      operationId: getRestAccountsContactsContactVcard
      x-api-path-slug: restaccountscontactscontactidvcard-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Get
      - Filestream
      - Of
      - Vcard
      - From
      - Customer
  /rest/boards/{boardId}/columns/{columnId}/tasks/{taskId}/references:
    post:
      summary: Creates a new reference from a given task to a contact or a ticket.
      description: Creates a new reference from a given task to a contact or a ticket..
      operationId: postRestBoardsBoardColumnsColumnTasksTaskReferences
      x-api-path-slug: restboardsboardidcolumnscolumnidtaskstaskidreferences-post
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: query
        name: referenceValue
        description: Reference type followed by foreign ID of the referenced object
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Reference
      - From
      - Given
      - Task
      - To
      - Contact
      - Ticket
  /rest/boards/{boardId}/columns/{columnId}/tasks/{taskId}/references/{referenceId}:
    delete:
      summary: Deletes a reference from a given task.
      description: Deletes a reference from a given task..
      operationId: deleteRestBoardsBoardColumnsColumnTasksTaskReferencesReference
      x-api-path-slug: restboardsboardidcolumnscolumnidtaskstaskidreferencesreferenceid-delete
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: path
        name: referenceId
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - S
      - Reference
      - From
      - Given
      - Task
  /rest/items/{id}/variations/{variationId}/variation_categories/{catId}:
    delete:
      summary: Remove a category from a variation
      description: Deletes the link between a category and a variation.
      operationId: deleteRestItemsVariationsVariationVariationCategoriesCat
      x-api-path-slug: restitemsidvariationsvariationidvariation-categoriescatid-delete
      parameters:
      - in: path
        name: catId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Category
      - From
      - Variation
  /rest/items/{id}/variations/{variationId}/variation_clients/{plentyId}:
    delete:
      summary: Unlink a client from a variation
      description: Deletes the link between a client (store) and a variation.
      operationId: deleteRestItemsVariationsVariationVariationClientsPlenty
      x-api-path-slug: restitemsidvariationsvariationidvariation-clientsplentyid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: plentyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Unlink
      - Client
      - From
      - Variation
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