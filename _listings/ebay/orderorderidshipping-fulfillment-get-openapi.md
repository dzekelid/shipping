---
swagger: "2.0"
x-collection-name: eBay
x-complete: 0
info:
  title: Ebay Get Order Order Shipping Fulfillment
  description: Use this call to retrieve the contents of all fulfillments currently
    defined for a specified order based on the order's unique identifier, orderId.
    This value is returned in the getOrders call's members.orderId field when you
    search for orders by creation date or shipment status.
  contact:
    name: eBay Inc.
  version: 1.0.0
host: api.ebay.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /order/{orderId}/shipping_fulfillment:
    get:
      summary: Get Order Order Shipping Fulfillment
      description: Use this call to retrieve the contents of all fulfillments currently
        defined for a specified order based on the order's unique identifier, orderId.
        This value is returned in the getOrders call's members.orderId field when
        you search for orders by creation date or shipment status.
      operationId: getShippingFulfillments
      x-api-path-slug: orderorderidshipping-fulfillment-get
      parameters:
      - in: path
        name: orderId
        description: The unique identifier of the order
      responses:
        200:
          description: OK
      tags:
      - Auctions
      - Order
      - Order
      - Shipping
      - Fulfillment
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