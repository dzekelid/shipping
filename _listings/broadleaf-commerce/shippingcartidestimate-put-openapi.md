---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 0
info:
  title: Broadleaf Commerce API Put Shipping Estimate
  description: Put shipping estimate.
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shipping/options:
    get:
      summary: Get Shipping Options
      description: Get shipping options.
      operationId: getShippingOptions
      x-api-path-slug: shippingoptions-get
      parameters:
      - in: query
        name: fulfillmentType
        description: fulfillmentType
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Options
  /shipping/{cartId}/estimate:
    get:
      summary: Get Shipping Estimate
      description: Get shipping estimate.
      operationId: getShippingCartEstimate
      x-api-path-slug: shippingcartidestimate-get
      parameters:
      - in: path
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Estimate
    head:
      summary: Head Shipping Estimate
      description: Head shipping estimate.
      operationId: headShippingCartEstimate
      x-api-path-slug: shippingcartidestimate-head
      parameters:
      - in: path
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Head
      - Shipping
      - Estimate
    post:
      summary: Post Shipping Estimate
      description: Post shipping estimate.
      operationId: postShippingCartEstimate
      x-api-path-slug: shippingcartidestimate-post
      parameters:
      - in: path
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Estimate
    put:
      summary: Put Shipping Estimate
      description: Put shipping estimate.
      operationId: putShippingCartEstimate
      x-api-path-slug: shippingcartidestimate-put
      parameters:
      - in: path
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Estimate
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