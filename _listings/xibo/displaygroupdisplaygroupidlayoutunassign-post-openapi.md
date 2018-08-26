---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Unassign one or more Layout items from a Display Group
  description: Removes the provided from the Display Group
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /displaygroup/{displayGroupId}/media/unassign:
    post:
      summary: Unassign one or more Media items from a Display Group
      description: Removes the provided from the Display Group
      operationId: displayGroupMediaUnassign
      x-api-path-slug: displaygroupdisplaygroupidmediaunassign-post
      parameters:
      - in: path
        name: displayGroupId
        description: The Display Group to unassign from
      - in: formData
        name: mediaId
        description: The Media Ids to unassign
      responses:
        200:
          description: OK
      tags:
      - Unassign
      - More
      - Media
      - Items
      - From
      - Display
      - Group
  /displaygroup/{displayGroupId}/layout/unassign:
    post:
      summary: Unassign one or more Layout items from a Display Group
      description: Removes the provided from the Display Group
      operationId: displayGroupLayoutUnassign
      x-api-path-slug: displaygroupdisplaygroupidlayoutunassign-post
      parameters:
      - in: path
        name: displayGroupId
        description: The Display Group to unassign from
      - in: formData
        name: layoutId
        description: The Layout Ids to unassign
      responses:
        200:
          description: OK
      tags:
      - Unassign
      - More
      - Layout
      - Items
      - From
      - Display
      - Group
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