---
swagger: "2.0"
info:
  title: Etsy Post Shipping Templates
  description: Creates a new ShippingTemplate
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shipping/templates:
    post:
      summary: Post Shipping Templates
      description: Creates a new ShippingTemplate
      operationId: postShippingTemplates
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
      - shipping
      - templates
definitions: []
x-collection-name: Etsy
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