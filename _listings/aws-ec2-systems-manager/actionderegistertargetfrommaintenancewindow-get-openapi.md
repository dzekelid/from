---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API Deregister Target From Maintenance Window
  version: 1.0.0
  description: Removes a target from a Maintenance Window.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeregisterTargetFromMaintenanceWindow:
    get:
      summary: Deregister Target From Maintenance Window
      description: Removes a target from a Maintenance Window.
      operationId: deregisterTargetFromMaintenanceWindow
      x-api-path-slug: actionderegistertargetfrommaintenancewindow-get
      parameters:
      - in: query
        name: WindowId
        description: The ID of the Maintenance Window the target should be removed
          from
        type: string
      - in: query
        name: WindowTargetId
        description: The ID of the target definition to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - Target
      - From
      - Maintenance
      - Window
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