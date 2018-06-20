---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shipping/providers:
    get:
      summary: Get Shipping Provers
      description: List of supported shipping providers
      operationId: getShippingProvers
      x-api-path-slug: shippingproviders-get
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Providers
  /shipping/regions:
    get:
      summary: Get Shipping Regions
      description: Get shipping regions.
      operationId: getShippingRegions
      x-api-path-slug: shippingregions-get
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Regions
  /shops/{shop_id}/shipping_profiles:
    get:
      summary: Get Shops Shop Shipping Profiles
      description: List of shipping profiles for your shop
      operationId: getShopsShopShippingProfiles
      x-api-path-slug: shopsshop-idshipping-profiles-get
      parameters:
      - in: path
        name: shop_id
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Shop
      - Id
      - Shipping
      - Profiles
---