---
swagger: "2.0"
x-collection-name: PayPal
x-complete: 0
info:
  title: Paypal Get Shipping Addresses
  description: Use the GetShippingAddresses API operation to obtain the selected shipping
    address. You must have created the payment or preapproval key that identifies
    the account holder whose shipping address you want to obtain, or be the primary
    receiver of the payment or one of the parallel receivers of the payment. The shipping
    address is available only if it was provided during the embedded payment flow.
  version: 1.0.0
host: svcs.sandbox.paypal.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /AdaptivePayments/GetShippingAddresses:
    post:
      summary: Get Shipping Addresses
      description: Use the GetShippingAddresses API operation to obtain the selected
        shipping address. You must have created the payment or preapproval key that
        identifies the account holder whose shipping address you want to obtain, or
        be the primary receiver of the payment or one of the parallel receivers of
        the payment. The shipping address is available only if it was provided during
        the embedded payment flow.
      operationId: AdaptivePayments.GetShippingAddresses.post
      x-api-path-slug: adaptivepaymentsgetshippingaddresses-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Addresses
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