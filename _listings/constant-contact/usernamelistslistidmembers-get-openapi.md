---
swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 0
info:
  title: Constant Contact Get Contacts Collection from a List
  description: Get Contacts Collection from a List
  version: 1.0.0
host: api.constantcontact.com
basePath: /ws/customers/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{username}/lists/{list-id}/members:
    get:
      summary: Get Contacts Collection from a List
      description: Get Contacts Collection from a List
      operationId: get-contacts-collection-from-a-list
      x-api-path-slug: usernamelistslistidmembers-get
      parameters:
      - in: path
        name: list-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Collection
      - From
      - List
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