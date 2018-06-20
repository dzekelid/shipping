---
name: Etsy
x-slug: etsy
description: Find handmade, vintage, and unique goods that express who you are.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
x-kinRank: "9"
x-alexaRank: "187"
tags: Shipping
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/etsy/apis.md
specificationVersion: "0.14"
apis:
- name: Etsy Get Listings Listing Shipping Info
  x-api-slug: etsy
  description: Retrieves a set of ShippingInfo objects associated to a Listing.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///listings/{listing_id}/shipping/info
  tags: Listings,Shipping,Info
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/etsy/listingslisting-idshippinginfo-get-openapi.md
- name: Etsy Post Listings Listing Shipping Info
  x-api-slug: etsy
  description: Creates a new ShippingInfo.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///listings/{listing_id}/shipping/info
  tags: Listings,Shipping,Info
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/etsy/listingslisting-idshippinginfo-post-openapi.md
- name: Etsy Get Shipping Info Shipping Info
  x-api-slug: etsy
  description: Retrieves a ShippingInfo by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///shipping/info/{shipping_info_id}
  tags: Shipping,Info,Shipping,Info
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/etsy/shippinginfoshipping-info-id-get-openapi.md
- name: Etsy Put Shipping Info Shipping Info
  x-api-slug: etsy
  description: Updates a ShippingInfo with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///shipping/info/{shipping_info_id}
  tags: Shipping,Info,Shipping,Info
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/etsy/shippinginfoshipping-info-id-put-openapi.md
- name: Etsy Delete Shipping Info Shipping Info
  x-api-slug: etsy
  description: Deletes the ShippingInfo with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///shipping/info/{shipping_info_id}
  tags: Shipping,Info,Shipping,Info
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/etsy/shippinginfoshipping-info-id-delete-openapi.md
- name: Etsy Get Shipping Templates Entries Shipping Template Entry
  x-api-slug: etsy
  description: Retrieves a ShippingTemplateEntry by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///shipping/templates/entries/{shipping_template_entry_id}
  tags: Shipping,Templates,Entries,Shipping,Template,Entry
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/etsy/shippingtemplatesentriesshipping-template-entry-id-get-openapi.md
- name: Etsy Put Shipping Templates Entries Shipping Template Entry
  x-api-slug: etsy
  description: Updates a ShippingTemplateEntry
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///shipping/templates/entries/{shipping_template_entry_id}
  tags: Shipping,Templates,Entries,Shipping,Template,Entry
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/etsy/shippingtemplatesentriesshipping-template-entry-id-put-openapi.md
- name: Etsy Delete Shipping Templates Entries Shipping Template Entry
  x-api-slug: etsy
  description: Deletes a ShippingTemplateEntry
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///shipping/templates/entries/{shipping_template_entry_id}
  tags: Shipping,Templates,Entries,Shipping,Template,Entry
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/etsy/shippingtemplatesentriesshipping-template-entry-id-delete-openapi.md
- name: Etsy Post Shipping Templates Entries
  x-api-slug: etsy
  description: Creates a new ShippingTemplateEntry
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///shipping/templates/entries
  tags: Shipping,Templates,Entries
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/etsy/shippingtemplatesentries-post-openapi.md
- name: Etsy Get Shipping Templates Shipping Template
  x-api-slug: etsy
  description: Retrieves a ShippingTemplate by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///shipping/templates/{shipping_template_id}
  tags: Shipping,Templates,Shipping,Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/etsy/shippingtemplatesshipping-template-id-get-openapi.md
- name: Etsy Delete Shipping Templates Shipping Template
  x-api-slug: etsy
  description: Deletes the ShippingTemplate with the given id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///shipping/templates/{shipping_template_id}
  tags: Shipping,Templates,Shipping,Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/etsy/shippingtemplatesshipping-template-id-delete-openapi.md
- name: Etsy Put Shipping Templates Shipping Template
  x-api-slug: etsy
  description: Updates a ShippingTemplate
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///shipping/templates/{shipping_template_id}
  tags: Shipping,Templates,Shipping,Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/etsy/shippingtemplatesshipping-template-id-put-openapi.md
- name: Etsy Get Shipping Templates Shipping Template Entries
  x-api-slug: etsy
  description: Retrieves a set of ShippingTemplateEntry objects associated to a ShippingTemplate.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///shipping/templates/{shipping_template_id}/entries
  tags: Shipping,Templates,Shipping,Template,Entries
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/etsy/shippingtemplatesshipping-template-identries-get-openapi.md
- name: Etsy Post Shipping Templates
  x-api-slug: etsy
  description: Creates a new ShippingTemplate
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///shipping/templates
  tags: Shipping,Templates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/etsy/shippingtemplates-post-openapi.md
- name: Etsy Get Users User Shipping Templates
  x-api-slug: etsy
  description: Retrieves a set of ShippingTemplate objects associated to a User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private///users/{user_id}/shipping/templates
  tags: Users,Shipping,Templates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/etsy/usersuser-idshippingtemplates-get-openapi.md
- name: Etsy
  x-api-slug: etsy
  description: Etsy is a handmade marketplace. The Etsy API lets developers tap into
    the Etsy community, building their own Etsy-powered applications for the web,
    desktop and mobile devices. Applications built on the API will connect buyers
    with sellers, promote the handmade lifestyle, and support the craftspeople who
    sell on Etsy.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/192-etsy.jpg
  humanURL: http://www.etsy.com/
  baseURL: https://openapi.etsy.com//v2/private/
  tags: Shipping
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/etsy/openapi.md
x-common:
- type: x-api-json--authoritative
  url: http://apis.io/apisdef/etsy.json
- type: x-application-gallery
  url: https://www.etsy.com/apps/
- type: x-base
  url: https://openapi.etsy.com/
- type: x-blog
  url: http://www.etsy.com/blog/en/
- type: x-blog-rss
  url: https://blog.etsy.com/en/feed/
- type: x-copyright
  url: https://www.etsy.com/help/article/482/?ref=ftr
- type: x-crunchbase
  url: https://crunchbase.com/organization/etsy
- type: x-crunchbase
  url: http://www.crunchbase.com/company/etsy
- type: x-developer
  url: https://www.etsy.com/developers/
- type: x-email
  url: enaffiliates@etsy.com
- type: x-email
  url: selleraffiliate@etsy.com
- type: x-email
  url: developer@etsy.com
- type: x-email
  url: legal@etsy.com
- type: x-email
  url: dpo@etsy.com
- type: x-email
  url: dispute-resolution@etsy.com
- type: x-forum
  url: https://www.etsy.com/developers/discussion
- type: x-github
  url: https://github.com/etsy
- type: x-privacy
  url: https://www.etsy.com/help/article/480/?ref=ftr
- type: x-terms-of-service
  url: https://www.etsy.com/help/article/479/?ref=ftr
- type: x-transparency-report
  url: http://blog.etsy.com/news/files/2015/07/Etsy_TransparencyReport_2014.pdf
- type: x-twitter
  url: https://twitter.com/Etsy
- type: x-website
  url: http://www.etsy.com/
- type: x-website
  url: http://etsy.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---