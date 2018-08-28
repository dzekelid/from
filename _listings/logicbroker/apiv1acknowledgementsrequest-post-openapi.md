---
swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 0
info:
  title: Logic Broker CommerceAPI Request an acknowledgement from a trading partner
  version: 1.0.0
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Shipments/Import:
    post:
      summary: Import from flat file.
      description: Request rate limited to 1 request per second with bursts up to
        10 requests.
      operationId: Shipment_Import
      x-api-path-slug: apiv1shipmentsimport-post
      parameters:
      - in: query
        name: aliases
        description: List of field names and aliases
      - in: query
        name: custom
        description: False for standard format, true if using custom mapping configured
          by Logicbroker
      - in: query
        name: delimiter
        description: Delimiter (CSV only)
      - in: query
        name: dryRun
        description: Return shipment list instead of saving
      - in: formData
        name: file
        description: File to import
      - in: query
        name: fileType
        description: CSV or XLSX
      responses:
        200:
          description: OK
      tags:
      - Import
      - From
      - Flat
      - File
  /api/v1/Returns/Import:
    post:
      summary: Import from flat file.
      description: Request rate limited to 1 request per second with bursts up to
        10 requests.
      operationId: Return_Import
      x-api-path-slug: apiv1returnsimport-post
      parameters:
      - in: query
        name: aliases
        description: List of field names and aliases
      - in: query
        name: custom
        description: False for standard format, true if using custom mapping configured
          by Logicbroker
      - in: query
        name: delimiter
        description: Delimiter (CSV only)
      - in: query
        name: dryRun
        description: Return shipment list instead of saving
      - in: formData
        name: file
        description: File to import
      - in: query
        name: fileType
        description: CSV or XLSX
      responses:
        200:
          description: OK
      tags:
      - Import
      - From
      - Flat
      - File
  /api/v1/Product/{partnerId}:
    post:
      summary: Import product from CSV.
      description: Request rate limited to 1 request per second with bursts up to
        10 requests.
      operationId: Product_Upload
      x-api-path-slug: apiv1productpartnerid-post
      parameters:
      - in: formData
        name: file
        description: File to import
      - in: path
        name: partnerId
        description: Partner account number
      responses:
        200:
          description: OK
      tags:
      - Import
      - Product
      - From
      - CSV
  /api/v1/Orders/Import:
    post:
      summary: Import from flat file.
      description: Request rate limited to 1 request per second with bursts up to
        10 requests.
      operationId: Order_Import
      x-api-path-slug: apiv1ordersimport-post
      parameters:
      - in: query
        name: aliases
        description: List of field names and aliases
      - in: query
        name: custom
        description: False for standard format, true if using custom mapping configured
          by Logicbroker
      - in: query
        name: delimiter
        description: Delimiter (CSV only)
      - in: query
        name: dryRun
        description: Return order list instead of saving
      - in: formData
        name: file
        description: File to import
      - in: query
        name: fileType
        description: CSV or XLSX
      responses:
        200:
          description: OK
      tags:
      - Import
      - From
      - Flat
      - File
  /api/v1/Invoices/Import:
    post:
      summary: Import from flat file.
      description: Request rate limited to 1 request per second with bursts up to
        10 requests.
      operationId: Invoice_Import
      x-api-path-slug: apiv1invoicesimport-post
      parameters:
      - in: query
        name: aliases
        description: List of field names and aliases
      - in: query
        name: custom
        description: False for standard format, true if using custom mapping configured
          by Logicbroker
      - in: query
        name: delimiter
        description: Delimiter (CSV only)
      - in: query
        name: dryRun
        description: Return invoice list instead of saving
      - in: formData
        name: file
        description: File to import
      - in: query
        name: fileType
        description: CSV or XLSX
      responses:
        200:
          description: OK
      tags:
      - Import
      - From
      - Flat
      - File
  /api/v1/Inventory/Broadcast:
    post:
      summary: Import inventory from CSV.
      description: Request rate limited to 1 request every 60 seconds with bursts
        up to 2 requests.
      operationId: Inventory_Broadcast
      x-api-path-slug: apiv1inventorybroadcast-post
      parameters:
      - in: formData
        name: file
        description: File to import
      - in: query
        name: transform
        description: Transform CSV (if configured)
      responses:
        200:
          description: OK
      tags:
      - Import
      - Inventory
      - From
      - CSV
  /api/v1/Inventory/{partnerId}:
    post:
      summary: Import inventory from CSV.
      description: Request rate limited to 1 request per second with bursts up to
        2 requests.
      operationId: Inventory_Upload
      x-api-path-slug: apiv1inventorypartnerid-post
      parameters:
      - in: formData
        name: file
        description: File to import
      - in: path
        name: partnerId
        description: Partner account number
      - in: query
        name: transform
        description: Transform CSV (if configured)
      responses:
        200:
          description: OK
      tags:
      - Import
      - Inventory
      - From
      - CSV
  /api/v1/Attachments/{container}/{name}:
    get:
      summary: Retrieve a file from Logicbroker storage.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Attachment_DownloadWithCoId
      x-api-path-slug: apiv1attachmentscontainername-get
      parameters:
      - in: path
        name: container
        description: File container (ex
      - in: path
        name: name
        description: File name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - File
      - From
      - Logicbroker
      - Storage
  /api/v1/Acknowledgements/Import:
    post:
      summary: Import from flat file.
      description: Request rate limited to 1 request per second with bursts up to
        10 requests.
      operationId: Acknowledgement_Import
      x-api-path-slug: apiv1acknowledgementsimport-post
      parameters:
      - in: query
        name: aliases
        description: List of field names and aliases
      - in: query
        name: custom
        description: False for standard format, true if using custom mapping configured
          by Logicbroker
      - in: query
        name: delimiter
        description: Delimiter (CSV only)
      - in: query
        name: dryRun
        description: Return shipment list instead of saving
      - in: formData
        name: file
        description: File to import
      - in: query
        name: fileType
        description: CSV or XLSX
      responses:
        200:
          description: OK
      tags:
      - Import
      - From
      - Flat
      - File
  /api/v1/Acknowledgements/Request:
    post:
      summary: Request an acknowledgement from a trading partner
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Acknowledgement_RequestAck
      x-api-path-slug: apiv1acknowledgementsrequest-post
      parameters:
      - in: body
        name: Acknowledgement
        description: Acknowledgement request object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Request
      - Acknowledgement
      - From
      - Trading
      - Partner
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