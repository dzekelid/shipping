swagger: "2.0"
x-collection-name: Etsy
x-complete: 1
info:
  title: Etsy
  description: bring-etsys-handmade-marketplace-and-community-into-your-apps-
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /listings/{listing_id}/shipping/info:
    get:
      summary: Get Listings Listing Shipping Info
      description: Retrieves a set of ShippingInfo objects associated to a Listing.
      operationId: getListingsListingShippingInfo
      x-api-path-slug: listingslisting-idshippinginfo-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: listing_id
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Shipping
      - Info
    post:
      summary: Post Listings Listing Shipping Info
      description: Creates a new ShippingInfo.
      operationId: postListingsListingShippingInfo
      x-api-path-slug: listingslisting-idshippinginfo-post
      parameters:
      - in: query
        name: destination_country_id
      - in: path
        name: listing_id
      - in: query
        name: origin_country_id
      - in: query
        name: primary_cost
      - in: query
        name: region_id
      - in: query
        name: secondary_cost
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Shipping
      - Info
  /shipping/info/{shipping_info_id}:
    get:
      summary: Get Shipping Info Shipping Info
      description: Retrieves a ShippingInfo by id.
      operationId: getShippingInfoShippingInfo
      x-api-path-slug: shippinginfoshipping-info-id-get
      parameters:
      - in: path
        name: shipping_info_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Info
      - Shipping
      - Info
    put:
      summary: Put Shipping Info Shipping Info
      description: Updates a ShippingInfo with the given id.
      operationId: putShippingInfoShippingInfo
      x-api-path-slug: shippinginfoshipping-info-id-put
      parameters:
      - in: query
        name: destination_country_id
      - in: query
        name: listing_id
      - in: query
        name: origin_country_id
      - in: query
        name: primary_cost
      - in: query
        name: region_id
      - in: query
        name: secondary_cost
      - in: path
        name: shipping_info_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Info
      - Shipping
      - Info
    delete:
      summary: Delete Shipping Info Shipping Info
      description: Deletes the ShippingInfo with the given id.
      operationId: deleteShippingInfoShippingInfo
      x-api-path-slug: shippinginfoshipping-info-id-delete
      parameters:
      - in: path
        name: shipping_info_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Info
      - Shipping
      - Info
  /shipping/templates/entries/{shipping_template_entry_id}:
    get:
      summary: Get Shipping Templates Entries Shipping Template Entry
      description: Retrieves a ShippingTemplateEntry by id.
      operationId: getShippingTemplatesEntriesShippingTemplateEntry
      x-api-path-slug: shippingtemplatesentriesshipping-template-entry-id-get
      parameters:
      - in: path
        name: shipping_template_entry_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Entries
      - Shipping
      - Template
      - Entry
    put:
      summary: Put Shipping Templates Entries Shipping Template Entry
      description: Updates a ShippingTemplateEntry
      operationId: putShippingTemplatesEntriesShippingTemplateEntry
      x-api-path-slug: shippingtemplatesentriesshipping-template-entry-id-put
      parameters:
      - in: query
        name: destination_country_id
      - in: query
        name: primary_cost
      - in: query
        name: secondary_cost
      - in: path
        name: shipping_template_entry_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Entries
      - Shipping
      - Template
      - Entry
    delete:
      summary: Delete Shipping Templates Entries Shipping Template Entry
      description: Deletes a ShippingTemplateEntry
      operationId: deleteShippingTemplatesEntriesShippingTemplateEntry
      x-api-path-slug: shippingtemplatesentriesshipping-template-entry-id-delete
      parameters:
      - in: path
        name: shipping_template_entry_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Entries
      - Shipping
      - Template
      - Entry
  /shipping/templates/entries:
    post:
      summary: Post Shipping Templates Entries
      description: Creates a new ShippingTemplateEntry
      operationId: postShippingTemplatesEntries
      x-api-path-slug: shippingtemplatesentries-post
      parameters:
      - in: query
        name: destination_country_id
      - in: query
        name: destination_region_id
      - in: query
        name: primary_cost
      - in: query
        name: secondary_cost
      - in: query
        name: shipping_template_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Entries
  /shipping/templates/{shipping_template_id}:
    get:
      summary: Get Shipping Templates Shipping Template
      description: Retrieves a ShippingTemplate by id.
      operationId: getShippingTemplatesShippingTemplate
      x-api-path-slug: shippingtemplatesshipping-template-id-get
      parameters:
      - in: path
        name: shipping_template_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Shipping
      - Template
    delete:
      summary: Delete Shipping Templates Shipping Template
      description: Deletes the ShippingTemplate with the given id.
      operationId: deleteShippingTemplatesShippingTemplate
      x-api-path-slug: shippingtemplatesshipping-template-id-delete
      parameters:
      - in: path
        name: shipping_template_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Shipping
      - Template
    put:
      summary: Put Shipping Templates Shipping Template
      description: Updates a ShippingTemplate
      operationId: putShippingTemplatesShippingTemplate
      x-api-path-slug: shippingtemplatesshipping-template-id-put
      parameters:
      - in: query
        name: origin_country_id
      - in: path
        name: shipping_template_id
      - in: query
        name: title
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Shipping
      - Template
  /shipping/templates/{shipping_template_id}/entries:
    get:
      summary: Get Shipping Templates Shipping Template Entries
      description: Retrieves a set of ShippingTemplateEntry objects associated to
        a ShippingTemplate.
      operationId: getShippingTemplatesShippingTemplateEntries
      x-api-path-slug: shippingtemplatesshipping-template-identries-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: shipping_template_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
      - Shipping
      - Template
      - Entries
  /shipping/templates:
    post:
      summary: Post Shipping Templates
      description: Creates a new ShippingTemplate
      operationId: postShippingTemplates
      x-api-path-slug: shippingtemplates-post
      parameters:
      - in: query
        name: destination_country_id
      - in: query
        name: destination_region_id
      - in: query
        name: origin_country_id
      - in: query
        name: primary_cost
      - in: query
        name: secondary_cost
      - in: query
        name: title
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Templates
  /users/{user_id}/shipping/templates:
    get:
      summary: Get Users User Shipping Templates
      description: Retrieves a set of ShippingTemplate objects associated to a User.
      operationId: getUsersUserShippingTemplates
      x-api-path-slug: usersuser-idshippingtemplates-get
      parameters:
      - in: query
        name: limit
        description: Bring Etsys handmade marketplace and community into your apps
      - in: query
        name: offset
        description: Bring Etsys handmade marketplace and community into your apps
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Shipping
      - Templates