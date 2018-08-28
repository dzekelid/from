swagger: "2.0"
x-collection-name: moltin
x-complete: 1
info:
  title: Moltin
  description: -welcomethis-is-a-place-to-put-general-notes-and-extra-information-for-internal-use-to-get-started-designingdocumenting-this-api-select-a-version-on-the-left-
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/carts/123456/items/{cartItemID}:
    delete:
      summary: Delete an item from a cart
      description: |-
        Delete an item from a cart. The remaining cart contents are returned on a successful delete.

        **Note:** `{item_id}` in the path is the identifier for the item in the cart rather than the product_id
      operationId: V2Carts123456ItemsByCartItemIDDelete
      x-api-path-slug: v2carts123456itemscartitemid-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cartItemID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Item
      - From
      - Cart