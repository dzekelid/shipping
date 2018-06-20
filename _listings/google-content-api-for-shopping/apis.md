---
name: Google Content API for Shopping
x-slug: google-content-api-for-shopping
description: 'API allowing retailers to manage their product feed content programmatically.
  Providing item-level data quality information: See if an item was disapproved because
  a landing page URL isn&rsquo;t working on a mobile device or if unique product identifiers
  are inaccurate. Faster pricing and availability updates: Ensure customers have the
  latest price-points and know what&rsquo;s in-stock before they click through to
  your site. More integration options: The newer API supports a broader choice of
  programming languages and data formats.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
x-kinRank: "9"
x-alexaRank: "0"
tags: Shipping
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/google-content-api-for-shopping/apis.md
specificationVersion: "0.14"
apis:
- name: Google Content API for Shopping API Shipping Settings
  x-api-slug: google-content-api-for-shopping-api
  description: Retrieves and updates the shipping settings of multiple accounts in
    a single request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2//shippingsettings/batch
  tags: Shipping, Settings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/google-content-api-for-shopping/shippingsettingsbatch-post-openapi.md
- name: Google Content API for Shopping API Get Account Shipping
  x-api-slug: google-content-api-for-shopping-api
  description: Lists the shipping settings of the sub-accounts in your Merchant Center
    account. This method can only be called for multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2//{merchantId}/accountshipping
  tags: Account, Shipping
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/google-content-api-for-shopping/merchantidaccountshipping-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/google-content-api-for-shopping/merchantidaccountshipping-get-openapi.md
- name: Google Content API for Shopping API Get Account Shipping
  x-api-slug: google-content-api-for-shopping-api
  description: 'Retrieves the shipping settings of the account. This method can only
    be called for accounts to which the managing account has access: either the managing
    account itself or sub-accounts if the managing account is a multi-client account.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2//{merchantId}/accountshipping/{accountId}
  tags: Account, Shipping
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/google-content-api-for-shopping/merchantidaccountshippingaccountid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/google-content-api-for-shopping/merchantidaccountshippingaccountid-get-openapi.md
- name: Google Content API for Shopping API Updat Account Shipping
  x-api-slug: google-content-api-for-shopping-api
  description: 'Updates the shipping settings of the account. This method can only
    be called for accounts to which the managing account has access: either the managing
    account itself or sub-accounts if the managing account is a multi-client account.
    This method supports patch semantics.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2//{merchantId}/accountshipping/{accountId}
  tags: Updat, Account, Shipping
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/google-content-api-for-shopping/merchantidaccountshippingaccountid-patch-openapi.md
- name: Google Content API for Shopping API Updat Account Shipping
  x-api-slug: google-content-api-for-shopping-api
  description: 'Updates the shipping settings of the account. This method can only
    be called for accounts to which the managing account has access: either the managing
    account itself or sub-accounts if the managing account is a multi-client account.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2//{merchantId}/accountshipping/{accountId}
  tags: Updat, Account, Shipping
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/google-content-api-for-shopping/merchantidaccountshippingaccountid-put-openapi.md
- name: Google Content API for Shopping API Get Shipping Settings
  x-api-slug: google-content-api-for-shopping-api
  description: Lists the shipping settings of the sub-accounts in your Merchant Center
    account. This method can only be called for multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2//{merchantId}/shippingsettings
  tags: Shipping, Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/google-content-api-for-shopping/merchantidshippingsettings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/google-content-api-for-shopping/merchantidshippingsettings-get-openapi.md
- name: Google Content API for Shopping API Get Shipping Settings
  x-api-slug: google-content-api-for-shopping-api
  description: 'Retrieves the shipping settings of the account. This method can only
    be called for accounts to which the managing account has access: either the managing
    account itself or sub-accounts if the managing account is a multi-client account.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2//{merchantId}/shippingsettings/{accountId}
  tags: Shipping, Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/google-content-api-for-shopping/merchantidshippingsettingsaccountid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/google-content-api-for-shopping/merchantidshippingsettingsaccountid-get-openapi.md
- name: Google Content API for Shopping API Update Shipping Settings
  x-api-slug: google-content-api-for-shopping-api
  description: 'Updates the shipping settings of the account. This method can only
    be called for accounts to which the managing account has access: either the managing
    account itself or sub-accounts if the managing account is a multi-client account.
    This method supports patch semantics.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2//{merchantId}/shippingsettings/{accountId}
  tags: Shipping, Settings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/google-content-api-for-shopping/merchantidshippingsettingsaccountid-patch-openapi.md
- name: Google Content API for Shopping API Update Shipping Settings
  x-api-slug: google-content-api-for-shopping-api
  description: 'Updates the shipping settings of the account. This method can only
    be called for accounts to which the managing account has access: either the managing
    account itself or sub-accounts if the managing account is a multi-client account.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2//{merchantId}/shippingsettings/{accountId}
  tags: Shipping, Settings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/google-content-api-for-shopping/merchantidshippingsettingsaccountid-put-openapi.md
- name: Google Content API for Shopping API
  x-api-slug: google-content-api-for-shopping-api
  description: 'API allowing retailers to manage their product feed content programmatically.
    Providing item-level data quality information: See if an item was disapproved
    because a landing page URL isn&rsquo;t working on a mobile device or if unique
    product identifiers are inaccurate. Faster pricing and availability updates: Ensure
    customers have the latest price-points and know what&rsquo;s in-stock before they
    click through to your site. More integration options: The newer API supports a
    broader choice of programming languages and data formats.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shipping
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/shipping/master/_listings/google-content-api-for-shopping/openapi.md
x-common:
- type: x-best-practices
  url: https://developers.google.com/shopping-content/v2/best-practices
- type: x-code
  url: https://developers.google.com/shopping-content/v2/libraries
- type: x-testing
  url: https://developers.google.com/shopping-content/v2/how-tos/testing
- type: x-website
  url: https://developers.google.com/shopping-content/v2/quickstart
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---