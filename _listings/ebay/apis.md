---
name: eBay
description: Buy and sell electronics, cars, fashion apparel, collectibles, sporting
  goods, digital cameras, baby items, coupons, and everything else on eBay, the worlds
  online marketplace.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/138_logo.png
x-kinRank: "8"
x-alexaRank: ""
tags:
- Stack
- Partners
- Commerce
- Auction
created: "2018-03-24"
modified: "2018-03-24"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/ebay/apis.yaml
specificationVersion: "0.14"
apis:
- name: Ebay
  description: Buy and sell electronics, cars, fashion apparel, collectibles, sporting
    goods, digital cameras, baby items, coupons, and everything else on eBay, the
    worlds online marketplace
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/138_logo.png
  humanURL: ""
  baseURL: https://api.ebay.com//
  tags: Shipping
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/ebay/order-orderid-shipping-fulfillment-fulfillmentid-get.md
- name: Ebay Get Order Order Shipping Fulfillment
  description: Use this call to retrieve the contents of all fulfillments currently
    defined for a specified order based on the order's unique identifier, orderId.
    This value is returned in the getOrders call's members.orderId field when you
    search for orders by creation date or shipment status.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/138_logo.png
  humanURL: https://ebay.com
  baseURL: https://api.ebay.com//
  tags: Shipping
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/ebay/order-orderid-shipping-fulfillment-get.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/ebay/order-orderid-shipping-fulfillment-get-postman.md
x-common:
- type: x-blog
  url: https://go.developer.ebay.com/dev-program-blog
- type: x-crunchbase
  url: http://www.crunchbase.com/company/ebay
- type: x-developer
  url: https://go.developer.ebay.com/
- type: x-github
  url: https://github.com/eBayDeveloper
- type: x-twitter
  url: https://twitter.com/ebaydev
- type: x-website
  url: https://ebay.com
- type: x-blog
  url: https://go.developer.ebay.com/dev-program-blog
- type: x-crunchbase
  url: http://www.crunchbase.com/company/ebay
- type: x-developer
  url: https://go.developer.ebay.com/
- type: x-github
  url: https://github.com/eBayDeveloper
- type: x-twitter
  url: https://twitter.com/ebaydev
- type: x-website
  url: https://ebay.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---