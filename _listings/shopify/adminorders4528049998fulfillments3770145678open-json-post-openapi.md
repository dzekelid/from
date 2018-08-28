---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Transition a fulfillment from pending to open.
  description: Transition a fulfillment from pending to open..
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/products/9579007950.json:
    delete:
      summary: Remove a product from the shop
      description: Remove a product from the shop.
      operationId: deleteAdminProducts9579007950.json
      x-api-path-slug: adminproducts9579007950-json-delete
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Remove
      - Product
      - From
      - Shop
  /admin/blogs/62581763/articles.json:
    get:
      summary: Get a list of all articles from a certain blog
      description: Get a list of all articles from a certain blog.
      operationId: getAdminBlogs62581763Articles.json
      x-api-path-slug: adminblogs62581763articles-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Articles
      - From
      - Certain
      - Blog
  /admin/orders/4554953422/events.json:
    get:
      summary: Get all the events from a particular order
      description: Get all the events from a particular order.
      operationId: getAdminOrders4554953422Events.json
      x-api-path-slug: adminorders4554953422events-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Events
      - From
      - Particular
      - Order
  /admin/blogs/62581763/articles/count.json:
    get:
      summary: Get a count of all articles from a certain blog
      description: Get a count of all articles from a certain blog.
      operationId: getAdminBlogs62581763ArticlesCount.json
      x-api-path-slug: adminblogs62581763articlescount-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Count
      - Articles
      - From
      - Certain
      - Blog
  /admin/orders/4554953422/refunds.json:
    get:
      summary: Get all refunds from a specific order
      description: Get all refunds from a specific order.
      operationId: getAdminOrders4554953422Refunds.json
      x-api-path-slug: adminorders4554953422refunds-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Refunds
      - From
      - Specific
      - Order
  /admin/orders.json:
    get:
      summary: Get all orders from a customer
      description: Get all orders from a customer.
      operationId: getAdminOrders.json
      x-api-path-slug: adminorders-json-get
      parameters:
      - in: header
        name: Content-Type
      - in: query
        name: customer_id
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Orders
      - From
      - Customer
  /admin/themes/110163843/assets.json:
    delete:
      summary: Remove assets from your shop
      description: Remove assets from your shop.
      operationId: deleteAdminThemes110163843Assets.json
      x-api-path-slug: adminthemes110163843assets-json-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Remove
      - Assets
      - From
      - Your
      - Shop
  /admin/orders/4528049998/fulfillments/3770145678/open.json:
    post:
      summary: Transition a fulfillment from pending to open.
      description: Transition a fulfillment from pending to open..
      operationId: postAdminOrders4528049998Fulfillments3770145678Open.json
      x-api-path-slug: adminorders4528049998fulfillments3770145678open-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Transition
      - Fulfillment
      - From
      - Pending
      - To
      - Open
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