swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/message/chat/{id}/{from}:
    get:
      summary: Get Message Chat From
      description: Get message chat from.
      operationId: getApiV1MessageChatFrom
      x-api-path-slug: apiv1messagechatidfrom-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: from
        description: "20"
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Message
      - Chat
      - From