swagger: "2.0"
x-collection-name: Google Content API for Shopping
x-complete: 1
info:
  title: Content API for Shopping
  description: manages-product-items-inventory-and-merchant-center-accounts-for-google-shopping-
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /content/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shippingsettings/batch:
    post:
      summary: Shipping Settings
      description: Retrieves and updates the shipping settings of multiple accounts
        in a single request.
      operationId: content.shippingsettings.custombatch
      x-api-path-slug: shippingsettingsbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Settings
  /{merchantId}/accountshipping:
    get:
      summary: Get Account Shipping
      description: Lists the shipping settings of the sub-accounts in your Merchant
        Center account. This method can only be called for multi-client accounts.
      operationId: content.accountshipping.list
      x-api-path-slug: merchantidaccountshipping-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of shipping settings to return in the response,
          used for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Account
      - Shipping
  /{merchantId}/accountshipping/{accountId}:
    get:
      summary: Get Account Shipping
      description: 'Retrieves the shipping settings of the account. This method can
        only be called for accounts to which the managing account has access: either
        the managing account itself or sub-accounts if the managing account is a multi-client
        account.'
      operationId: content.accountshipping.get
      x-api-path-slug: merchantidaccountshippingaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update account shipping
          settings
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Account
      - Shipping
    patch:
      summary: Updat Account Shipping
      description: 'Updates the shipping settings of the account. This method can
        only be called for accounts to which the managing account has access: either
        the managing account itself or sub-accounts if the managing account is a multi-client
        account. This method supports patch semantics.'
      operationId: content.accountshipping.patch
      x-api-path-slug: merchantidaccountshippingaccountid-patch
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update account shipping
          settings
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Updat
      - Account
      - Shipping
    put:
      summary: Updat Account Shipping
      description: 'Updates the shipping settings of the account. This method can
        only be called for accounts to which the managing account has access: either
        the managing account itself or sub-accounts if the managing account is a multi-client
        account.'
      operationId: content.accountshipping.update
      x-api-path-slug: merchantidaccountshippingaccountid-put
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update account shipping
          settings
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Updat
      - Account
      - Shipping
  /{merchantId}/shippingsettings:
    get:
      summary: Get Shipping Settings
      description: Lists the shipping settings of the sub-accounts in your Merchant
        Center account. This method can only be called for multi-client accounts.
      operationId: content.shippingsettings.list
      x-api-path-slug: merchantidshippingsettings-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of shipping settings to return in the response,
          used for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Settings
  /{merchantId}/shippingsettings/{accountId}:
    get:
      summary: Get Shipping Settings
      description: 'Retrieves the shipping settings of the account. This method can
        only be called for accounts to which the managing account has access: either
        the managing account itself or sub-accounts if the managing account is a multi-client
        account.'
      operationId: content.shippingsettings.get
      x-api-path-slug: merchantidshippingsettingsaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update shipping settings
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Settings
    patch:
      summary: Update Shipping Settings
      description: 'Updates the shipping settings of the account. This method can
        only be called for accounts to which the managing account has access: either
        the managing account itself or sub-accounts if the managing account is a multi-client
        account. This method supports patch semantics.'
      operationId: content.shippingsettings.patch
      x-api-path-slug: merchantidshippingsettingsaccountid-patch
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update shipping settings
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Settings
    put:
      summary: Update Shipping Settings
      description: 'Updates the shipping settings of the account. This method can
        only be called for accounts to which the managing account has access: either
        the managing account itself or sub-accounts if the managing account is a multi-client
        account.'
      operationId: content.shippingsettings.update
      x-api-path-slug: merchantidshippingsettingsaccountid-put
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update shipping settings
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Settings