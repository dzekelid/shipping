swagger: "2.0"
x-collection-name: PayPal
x-complete: 1
info:
  title: PayPal (Sandbox)
  description: bring-payments-to-apps-mobile-and-social-with-adaptive-payments-bsandbox-api-b
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