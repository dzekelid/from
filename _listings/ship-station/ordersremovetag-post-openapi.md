---
swagger: "2.0"
x-collection-name: Ship Station
x-complete: 0
info:
  title: Ship Station Remove Tag from Order
  description: |-
    Removes a tag from the specified order.  The body of this request has the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderId`` | number, required | Identifies the order whose tag will be removed.
    ``tagId`` | number, required | Identifies the tag to remove.
  version: 1.0.0
host: ssapi.shipstation.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders/removetag:
    post:
      summary: Remove Tag from Order
      description: |-
        Removes a tag from the specified order.  The body of this request has the following attributes:

        Name               |Data Type          |Description
        -------------------|-------------------|-------------------
        ``orderId`` | number, required | Identifies the order whose tag will be removed.
        ``tagId`` | number, required | Identifies the tag to remove.
      operationId: orders.removetag.post
      x-api-path-slug: ordersremovetag-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Tag
      - From
      - Order
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