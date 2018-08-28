swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 1
info:
  title: CommerceAPI
  version: 1.0.0
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Shipments/{LogicbrokerKey}/ShippingLabel:
    get:
      summary: Get shipping labels for one shipment.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Shipment_GetShipmentShippingSingleLabelToken
      x-api-path-slug: apiv1shipmentslogicbrokerkeyshippinglabel-get
      parameters:
      - in: query
        name: containerCode
        description: Specific container code
      - in: query
        name: fileType
        description: 'Valid types: jpg, png, pdf, ps, zpl'
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      - in: query
        name: ViewInBrowser
        description: Set to true to view the resulting link in the browser
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Labelsone
      - Shipment
  /api/v1/Shipments/ShippingLabel:
    post:
      summary: Get shipping labels for a shipment before submitting
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Shipment_GetShipmentShippingLabelToken
      x-api-path-slug: apiv1shipmentsshippinglabel-post
      parameters:
      - in: query
        name: containerCode
        description: Specific container code
      - in: query
        name: fileType
        description: 'Valid types: jpg, png, pdf, ps, zpl'
      - in: body
        name: shipment
        description: Shipment data
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: ViewInBrowser
        description: Set to true to view the resulting link in the browser
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Labelsa
      - Shipment
      - Before
      - Submitting
    get:
      summary: Get shipping labels for multiple shipments
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Shipment_GetShipmentShippingLabelToken
      x-api-path-slug: apiv1shipmentsshippinglabel-get
      parameters:
      - in: query
        name: containerCode
        description: Specific container code
      - in: query
        name: fileType
        description: 'Valid types: jpg, png, pdf, ps, zpl'
      - in: query
        name: LogicbrokerKeys
        description: The Logicbroker keys
      - in: query
        name: ViewInBrowser
        description: Set to true to view the resulting link in the browser
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Labelsmultiple
      - Shipments
  /api/v1/Orders/{LogicbrokerKey}/ShippingOptions:
    get:
      summary: Get shipping/tracking label options.
      description: Request rate limited to 2 requests per second with bursts up to
        25 requests.
      operationId: Order_GetShippingOptions
      x-api-path-slug: apiv1orderslogicbrokerkeyshippingoptions-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Tracking
      - Label
      - Options