---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List files from frontend storage. Append public cloudfront
    url to each retrieved object.
  description: List files from frontend storage. append public cloudfront url to each
    retrieved object..
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
  /rest/orders/items/dates/{id}:
    delete:
      summary: Delete a date from an order item
      description: Deletes the date from an order item. The ID of the date must be
        specified.
      operationId: deleteRestOrdersItemsDates
      x-api-path-slug: restordersitemsdatesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Date
      - From
      - Order
      - Item
  /rest/orders/items/{orderItemId}/dates/{typeId}:
    delete:
      summary: Delete a date from an order item by order item and date type
      description: Deletest a date from an order item. The ID of the order item and
        the ID of the date type must be specified.
      operationId: deleteRestOrdersItemsOrderitemDatesType
      x-api-path-slug: restordersitemsorderitemiddatestypeid-delete
      parameters:
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Date
      - From
      - Order
      - Item
      - By
      - Order
      - Item
      - Date
      - Type
  /rest/plugin_sets/{setId}/plugins/{pluginId}:
    delete:
      summary: Remove a plugin from a set
      description: |-
        Removes a plugin from a set and deletes all plugin files. Response content will be 'true' if the deletion was successful,
        'false' if not. If no plugin set with the given id can be found or the plugin is not associated to the set, a 404 will be returned.
      operationId: deleteRestPluginSetsSetPluginsPlugin
      x-api-path-slug: restplugin-setssetidpluginspluginid-delete
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Plugin
      - From
      - Set
  /rest/properties/groups/surcharge/types:
    get:
      summary: Get surcharge types from module configuration
      description: Get surcharge types from module configuration.
      operationId: getRestPropertiesGroupsSurchargeTypes
      x-api-path-slug: restpropertiesgroupssurchargetypes-get
      responses:
        200:
          description: OK
      tags:
      - Surcharge
      - Types
      - From
      - Module
      - Configuration
  /rest/properties/groups/types:
    get:
      summary: Get group types from module configuration
      description: Get group types from module configuration.
      operationId: getRestPropertiesGroupsTypes
      x-api-path-slug: restpropertiesgroupstypes-get
      responses:
        200:
          description: OK
      tags:
      - Group
      - Types
      - From
      - Module
      - Configuration
  /rest/properties/groups/{groupId}/properties/{propertyId}:
    delete:
      summary: Detach a property from a property group.
      description: Detaches a property from a property group. The ID of the property
        and the ID of the property group must be specified.
      operationId: deleteRestPropertiesGroupsGroupPropertiesProperty
      x-api-path-slug: restpropertiesgroupsgroupidpropertiespropertyid-delete
      parameters:
      - in: path
        name: groupId
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Detach
      - Property
      - From
      - Property
      - Group
  /rest/shop_builder/pages:
    get:
      summary: List content pages from all plugins in a given plugin set.
      description: List content pages from all plugins in a given plugin set..
      operationId: getRestShopBuilderPages
      x-api-path-slug: restshop-builderpages-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Content
      - Pages
      - From
      - ""
      - Plugins
      - In
      - Given
      - Plugin
      - Set
  /rest/storage/frontend/file:
    delete:
      summary: Remove a single object from frontend storage.
      description: Remove a single object from frontend storage..
      operationId: deleteRestStorageFrontendFile
      x-api-path-slug: reststoragefrontendfile-delete
      parameters:
      - in: query
        name: key
        description: The key of the object to delete
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Single
      - Object
      - From
      - Frontend
      - Storage
  /rest/storage/frontend/files:
    delete:
      summary: Delete files from frontend storage.
      description: Deletes a list of files from frontend storage. A list of storage
        keys must be specified.
      operationId: deleteRestStorageFrontendFiles
      x-api-path-slug: reststoragefrontendfiles-delete
      parameters:
      - in: query
        name: keyList
        description: List of storage keys for the files to be deleted
      responses:
        200:
          description: OK
      tags:
      - Files
      - From
      - Frontend
      - Storage
    get:
      summary: List files from frontend storage. Append public cloudfront url to each
        retrieved object.
      description: List files from frontend storage. append public cloudfront url
        to each retrieved object..
      operationId: getRestStorageFrontendFiles
      x-api-path-slug: reststoragefrontendfiles-get
      parameters:
      - in: query
        name: continuationToken
        description: The continuationToken of a previous request to continue listing
          objects with
      responses:
        200:
          description: OK
      tags:
      - List
      - Files
      - From
      - Frontend
      - Storage
      - ""
      - Append
      - Public
      - Cloudfront
      - Url
      - To
      - Each
      - Retrieved
      - Object
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