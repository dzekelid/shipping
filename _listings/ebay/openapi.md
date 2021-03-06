swagger: "2.0"
x-collection-name: eBay
x-complete: 1
info:
  title: Ebay
  description: the-ebay-platform-offers-an-unprecedented-opportunity-to-build-a-new-ebay-business-or-expand-your-current-business-reach-new-customers-and-create-a-potential-new-stream-of-revenue--leverage-the-resources-of-the-ebay-developers-program-to-tap-into-the-ebay-marketplace-with-millions-of-active-users-globally-with-tools-and-services-that-meet-the-diverse-needs-of-buyers-and-sellers-
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
    post:
      summary: Add Order Order Shipping Fulfillment
      description: 'When you group an order''s line items into one or more packages,
        each package requires a corresponding plan for handling, addressing, and shipping;
        this is a shipping fulfillment. For each package, execute this call once to
        generate a shipping fulfillment associated with that package. Note: A single
        line item in an order can consist of multiple units of a purchased item, and
        one unit can consist of multiple parts or components. Although these components
        might be provided by the manufacturer in separate packaging, the seller must
        include all components of a given line item in the same package.Before using
        this call for a given package, you must determine which line items are in
        the package. If the package has been shipped, you should provide the date
        of shipment in the request. If not provided, it will default to the current
        date and time.'
      operationId: createShippingFulfillment
      x-api-path-slug: orderorderidshipping-fulfillment-post
      parameters:
      - in: body
        name: body
        description: fulfillment payload
        schema:
          $ref: '#/definitions/holder'
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
  /order/{orderId}/shipping_fulfillment/{fulfillmentId}:
    get:
      summary: Get Order Order Shipping Fulfillment Fulfillment
      description: Use this call to retrieve the contents of a fulfillment based on
        its unique identifier, fulfillmentId (combined with the associated order's
        orderId). The fulfillmentId value was originally generated by the createShippingFulfillment
        call, and is returned by the getShippingFulfillments call in the members.fulfillmentId
        field.
      operationId: getShippingFulfillment
      x-api-path-slug: orderorderidshipping-fulfillmentfulfillmentid-get
      parameters:
      - in: path
        name: fulfillmentId
        description: The unique identifier of the fulfillment
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
      - Fulfillment