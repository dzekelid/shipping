---
swagger: "2.0"
x-collection-name: NxtPort
x-complete: 0
info:
  title: Portcall+ API Get Vessels In Port
  description: Get all the in-port vessels of BEANR and BEZEE
  version: 1.0.0
host: api-sb.nxtport.eu
basePath: /PortCallPlus/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /stays/{imoNumber}:
    get:
      summary: Get Stay
      description: Get a single stay by IMO number.
      operationId: Stays By ImoNumber
      x-api-path-slug: staysimonumber-get
      parameters:
      - in: path
        name: imoNumber
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Stays
  /nxtportdocument/{bookingnumber}/{containernumber}:
    get:
      summary: Get VERMAS Files
      description: Returns the VERMAS files with the according booking number and
        container number
      operationId: NxtportdocumentByBookingnumberByContainernumberGet
      x-api-path-slug: nxtportdocumentbookingnumbercontainernumber-get
      parameters:
      - in: path
        name: bookingnumber
        description: bookingnumber
      - in: path
        name: containernumber
        description: containernumber
      - in: header
        name: Ocp-Apim-Subscription-Key
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - VERMAS
      - Files
  /vessels/expected:
    get:
      summary: Get Expected Vessels
      description: Get all the expected vessels of BEANR and BEZEE
      operationId: Vessels_Expected
      x-api-path-slug: vesselsexpected-get
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Vessels
      - Ports
  /vessels/in-port:
    get:
      summary: Get Vessels In Port
      description: Get all the in-port vessels of BEANR and BEZEE
      operationId: Vessels_InPort
      x-api-path-slug: vesselsinport-get
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Vesses
      - Ports
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