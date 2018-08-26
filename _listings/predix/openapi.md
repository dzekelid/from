---
swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /decks/{id}/cards/remove:
    post:
      summary: Remove Cards from Deck
      description: Remove cards from deck.
      operationId: postDecksCardsRemove
      x-api-path-slug: decksidcardsremove-post
      parameters:
      - in: body
        name: cardIds
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Cards
      - From
      - Deck
---