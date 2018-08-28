---
swagger: "2.0"
x-collection-name: Digital River
x-complete: 0
info:
  title: Digital River Shopper API Get Shoppers Me Carts Active Shipping Options
  description: Get shoppers me carts active shipping options.
  version: v1
host: store.digitalriver.com
basePath: /store/{mysite}
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/shoppers/me/carts/active/apply-shipping-option:
    post:
      summary: Post Shoppers Me Carts Active Apply Shipping Option
      description: Post shoppers me carts active apply shipping option.
      operationId: postV1ShoppersMeCartsActiveApplyShippingOption
      x-api-path-slug: v1shoppersmecartsactiveapplyshippingoption-post
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Apply
      - Shipping
      - Option
  /v1/shoppers/me/carts/active/shipping-address:
    get:
      summary: Get Shoppers Me Carts Active Shipping Address
      description: Get shoppers me carts active shipping address.
      operationId: getV1ShoppersMeCartsActiveShippingAddress
      x-api-path-slug: v1shoppersmecartsactiveshippingaddress-get
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Shipping
      - Ress
    put:
      summary: Put Shoppers Me Carts Active Shipping Address
      description: Put shoppers me carts active shipping address.
      operationId: putV1ShoppersMeCartsActiveShippingAddress
      x-api-path-slug: v1shoppersmecartsactiveshippingaddress-put
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Shipping
      - Ress
  /v1/shoppers/me/carts/active/shipping-options:
    get:
      summary: Get Shoppers Me Carts Active Shipping Options
      description: Get shoppers me carts active shipping options.
      operationId: getV1ShoppersMeCartsActiveShippingOptions
      x-api-path-slug: v1shoppersmecartsactiveshippingoptions-get
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Shipping
      - Options
  /v1/shoppers/me/carts/active/shipping-options/{id}:
    get:
      summary: Get Shoppers Me Carts Active Shipping Options
      description: Get shoppers me carts active shipping options.
      operationId: getV1ShoppersMeCartsActiveShippingOptions
      x-api-path-slug: v1shoppersmecartsactiveshippingoptionsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Carts
      - Active
      - Shipping
      - Options
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