---
swagger: "2.0"
x-collection-name: Square
x-complete: 0
info:
  title: Square Connect API Deletes a cell from a Favorites page in Square Register.
  description: Deletes a cell from a Favorites page in Square Register.
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/me/timecards/{timecard_id}:
    delete:
      summary: Deletes a timecard. Deleted timecards are still accessible from Connect
        API endpoints, but the value of their deleted field is set to true. See Handling
        deleted timecards for more information.
      description: Deletes a timecard. Deleted timecards are still accessible from
        Connect API endpoints, but the value of their deleted field is set to true.
        See Handling deleted timecards for more information.
      operationId: DeleteTimecard
      x-api-path-slug: v1metimecardstimecard-id-delete
      parameters:
      - in: path
        name: timecard_id
        description: The ID of the timecard to delete
      responses:
        200:
          description: OK
      tags:
      - S
      - Timecard
      - ""
      - D
      - Timecards
      - Are
      - Still
      - Accessible
      - From
      - Connect
      - Endpoints
      - ""
      - But
      - Value
      - Of
      - Their
      - Deleted
      - Field
      - Is
      - Set
      - To
      - "True"
      - ""
      - See
      - Handling
      - Deleted
      - Timecardsmore
      - Information
  /v1/{location_id}/items/{item_id}/fees/{fee_id}:
    delete:
      summary: Removes a fee assocation from an item, meaning the fee is no longer
        automatically applied to the item in Square Register.
      description: Removes a fee assocation from an item, meaning the fee is no longer
        automatically applied to the item in Square Register.
      operationId: RemoveFee
      x-api-path-slug: v1location-iditemsitem-idfeesfee-id-delete
      parameters:
      - in: path
        name: fee_id
        description: The ID of the fee to apply
      - in: path
        name: item_id
        description: The ID of the item to add the fee to
      - in: path
        name: location_id
        description: The ID of the fees associated location
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Fee
      - Assocation
      - From
      - Item
      - ""
      - Meaning
      - Fee
      - Is
      - "No"
      - Longer
      - Automatically
      - Applied
      - To
      - Item
      - In
      - Square
      - Register
  /v1/{location_id}/items/{item_id}/modifier-lists/{modifier_list_id}:
    delete:
      summary: Removes a modifier list association from an item, meaning modifier
        options from the list can no longer be applied to the item.
      description: Removes a modifier list association from an item, meaning modifier
        options from the list can no longer be applied to the item.
      operationId: RemoveModifierList
      x-api-path-slug: v1location-iditemsitem-idmodifierlistsmodifier-list-id-delete
      parameters:
      - in: path
        name: item_id
        description: The ID of the item to remove the modifier list from
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to remove
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Modifier
      - List
      - Association
      - From
      - Item
      - ""
      - Meaning
      - Modifier
      - Options
      - From
      - List
      - Can
      - "No"
      - Longer
      - Be
      - Applied
      - To
      - Item
    put:
      summary: Associates a modifier list with an item, meaning modifier options from
        the list can be applied to the item.
      description: Associates a modifier list with an item, meaning modifier options
        from the list can be applied to the item.
      operationId: ApplyModifierList
      x-api-path-slug: v1location-iditemsitem-idmodifierlistsmodifier-list-id-put
      parameters:
      - in: path
        name: item_id
        description: The ID of the item to add the modifier list to
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to apply
      responses:
        200:
          description: OK
      tags:
      - Associates
      - Modifier
      - List
      - Item
      - ""
      - Meaning
      - Modifier
      - Options
      - From
      - List
      - Can
      - Be
      - Applied
      - To
      - Item
  /v1/{location_id}/items/{item_id}/variations/{variation_id}:
    delete:
      summary: Deletes an existing item variation from an item.
      description: Deletes an existing item variation from an item.
      operationId: DeleteVariation
      x-api-path-slug: v1location-iditemsitem-idvariationsvariation-id-delete
      parameters:
      - in: path
        name: item_id
        description: The ID of the item to delete
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: variation_id
        description: The ID of the variation to delete
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Item
      - Variation
      - From
      - Item
  /v1/{location_id}/modifier-lists/{modifier_list_id}/modifier-options/{modifier_option_id}:
    delete:
      summary: Deletes an existing item modifier option from a modifier list.
      description: Deletes an existing item modifier option from a modifier list.
      operationId: DeleteModifierOption
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-idmodifieroptionsmodifier-option-id-delete
      parameters:
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to delete
      - in: path
        name: modifier_option_id
        description: The ID of the modifier list to edit
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Item
      - Modifier
      - Option
      - From
      - Modifier
      - List
  /v1/{location_id}/pages/{page_id}/cells:
    delete:
      summary: Deletes a cell from a Favorites page in Square Register.
      description: Deletes a cell from a Favorites page in Square Register.
      operationId: DeletePageCell
      x-api-path-slug: v1location-idpagespage-idcells-delete
      parameters:
      - in: query
        name: column
        description: The column of the cell to clear
      - in: path
        name: location_id
        description: The ID of the Favorites pages associated location
      - in: path
        name: page_id
        description: The ID of the page to delete
      - in: query
        name: row
        description: The row of the cell to clear
      responses:
        200:
          description: OK
      tags:
      - S
      - Cell
      - From
      - Favorites
      - Page
      - In
      - Square
      - Register
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