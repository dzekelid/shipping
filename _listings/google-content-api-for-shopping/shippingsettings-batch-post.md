---
swagger: "2.0"
info:
  title: Content API for Shopping
  description: Manages product items, inventory, and Merchant Center accounts for
    Google Shopping.
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
        in a single request
      operationId: content.shippingsettings.custombatch
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
      - shipping
      - settings
definitions:
  Account:
    properties:
      adultContent:
        description: This is a default description.
        type: parameters
      adwordsLinks:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      reviewsUrl:
        description: This is a default description.
        type: parameters
      sellerId:
        description: This is a default description.
        type: parameters
      users:
        description: This is a default description.
        type: parameters
      websiteUrl:
        description: This is a default description.
        type: parameters
  AccountAdwordsLink:
    properties:
      adwordsId:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
  AccountIdentifier:
    properties:
      aggregatorId:
        description: This is a default description.
        type: parameters
      merchantId:
        description: This is a default description.
        type: parameters
  AccountShipping:
    properties:
      accountId:
        description: This is a default description.
        type: parameters
      carrierRates:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      locationGroups:
        description: This is a default description.
        type: parameters
      rateTables:
        description: This is a default description.
        type: parameters
      services:
        description: This is a default description.
        type: parameters
  AccountShippingCarrierRate:
    properties:
      carrier:
        description: This is a default description.
        type: parameters
      carrierService:
        description: This is a default description.
        type: parameters
      modifierPercent:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      saleCountry:
        description: This is a default description.
        type: parameters
      shippingOrigin:
        description: This is a default description.
        type: parameters
  AccountShippingCondition:
    properties:
      deliveryLocationGroup:
        description: This is a default description.
        type: parameters
      deliveryLocationId:
        description: This is a default description.
        type: parameters
      deliveryPostalCode:
        description: This is a default description.
        type: parameters
      shippingLabel:
        description: This is a default description.
        type: parameters
  AccountShippingLocationGroup:
    properties:
      country:
        description: This is a default description.
        type: parameters
      locationIds:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      postalCodeRanges:
        description: This is a default description.
        type: parameters
      postalCodes:
        description: This is a default description.
        type: parameters
  AccountShippingPostalCodeRange:
    properties:
      end:
        description: This is a default description.
        type: parameters
      start:
        description: This is a default description.
        type: parameters
  AccountShippingRateTable:
    properties:
      content:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      saleCountry:
        description: This is a default description.
        type: parameters
  AccountShippingRateTableCell:
    properties: []
  AccountShippingShippingService:
    properties:
      active:
        description: This is a default description.
        type: parameters
      maxDaysInTransit:
        description: This is a default description.
        type: parameters
      minDaysInTransit:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      saleCountry:
        description: This is a default description.
        type: parameters
  AccountShippingShippingServiceCalculationMethod:
    properties:
      carrierRate:
        description: This is a default description.
        type: parameters
      excluded:
        description: This is a default description.
        type: parameters
      percentageRate:
        description: This is a default description.
        type: parameters
      rateTable:
        description: This is a default description.
        type: parameters
  AccountShippingShippingServiceCostRule:
    properties:
      children:
        description: This is a default description.
        type: parameters
  AccountStatus:
    properties:
      accountId:
        description: This is a default description.
        type: parameters
      dataQualityIssues:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  AccountStatusDataQualityIssue:
    properties:
      country:
        description: This is a default description.
        type: parameters
      detail:
        description: This is a default description.
        type: parameters
      displayedValue:
        description: This is a default description.
        type: parameters
      exampleItems:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      lastChecked:
        description: This is a default description.
        type: parameters
      location:
        description: This is a default description.
        type: parameters
      numItems:
        description: This is a default description.
        type: parameters
      severity:
        description: This is a default description.
        type: parameters
      submittedValue:
        description: This is a default description.
        type: parameters
  AccountStatusExampleItem:
    properties:
      itemId:
        description: This is a default description.
        type: parameters
      link:
        description: This is a default description.
        type: parameters
      submittedValue:
        description: This is a default description.
        type: parameters
      title:
        description: This is a default description.
        type: parameters
      valueOnLandingPage:
        description: This is a default description.
        type: parameters
  AccountTax:
    properties:
      accountId:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      rules:
        description: This is a default description.
        type: parameters
  AccountTaxTaxRule:
    properties:
      country:
        description: This is a default description.
        type: parameters
      locationId:
        description: This is a default description.
        type: parameters
      ratePercent:
        description: This is a default description.
        type: parameters
      shippingTaxed:
        description: This is a default description.
        type: parameters
      useGlobalRate:
        description: This is a default description.
        type: parameters
  AccountUser:
    properties:
      admin:
        description: This is a default description.
        type: parameters
      emailAddress:
        description: This is a default description.
        type: parameters
  AccountsAuthInfoResponse:
    properties:
      accountIdentifiers:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  AccountsCustomBatchRequest:
    properties:
      entries:
        description: This is a default description.
        type: parameters
  AccountsCustomBatchRequestEntry:
    properties:
      accountId:
        description: This is a default description.
        type: parameters
      batchId:
        description: This is a default description.
        type: parameters
      merchantId:
        description: This is a default description.
        type: parameters
      method:
        description: This is a default description.
        type: parameters
  AccountsCustomBatchResponse:
    properties:
      entries:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  AccountsCustomBatchResponseEntry:
    properties:
      batchId:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  AccountsListResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      resources:
        description: This is a default description.
        type: parameters
  AccountshippingCustomBatchRequest:
    properties:
      entries:
        description: This is a default description.
        type: parameters
  AccountshippingCustomBatchRequestEntry:
    properties:
      accountId:
        description: This is a default description.
        type: parameters
      batchId:
        description: This is a default description.
        type: parameters
      merchantId:
        description: This is a default description.
        type: parameters
      method:
        description: This is a default description.
        type: parameters
  AccountshippingCustomBatchResponse:
    properties:
      entries:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  AccountshippingCustomBatchResponseEntry:
    properties:
      batchId:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  AccountshippingListResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      resources:
        description: This is a default description.
        type: parameters
  AccountstatusesCustomBatchRequest:
    properties:
      entries:
        description: This is a default description.
        type: parameters
  AccountstatusesCustomBatchRequestEntry:
    properties:
      accountId:
        description: This is a default description.
        type: parameters
      batchId:
        description: This is a default description.
        type: parameters
      merchantId:
        description: This is a default description.
        type: parameters
      method:
        description: This is a default description.
        type: parameters
  AccountstatusesCustomBatchResponse:
    properties:
      entries:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  AccountstatusesCustomBatchResponseEntry:
    properties:
      batchId:
        description: This is a default description.
        type: parameters
  AccountstatusesListResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      resources:
        description: This is a default description.
        type: parameters
  AccounttaxCustomBatchRequest:
    properties:
      entries:
        description: This is a default description.
        type: parameters
  AccounttaxCustomBatchRequestEntry:
    properties:
      accountId:
        description: This is a default description.
        type: parameters
      batchId:
        description: This is a default description.
        type: parameters
      merchantId:
        description: This is a default description.
        type: parameters
      method:
        description: This is a default description.
        type: parameters
  AccounttaxCustomBatchResponse:
    properties:
      entries:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  AccounttaxCustomBatchResponseEntry:
    properties:
      batchId:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  AccounttaxListResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      resources:
        description: This is a default description.
        type: parameters
  CarrierRate:
    properties:
      carrierName:
        description: This is a default description.
        type: parameters
      carrierService:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      originPostalCode:
        description: This is a default description.
        type: parameters
      percentageAdjustment:
        description: This is a default description.
        type: parameters
  CarriersCarrier:
    properties:
      country:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      services:
        description: This is a default description.
        type: parameters
  Datafeed:
    properties:
      attributeLanguage:
        description: This is a default description.
        type: parameters
      contentLanguage:
        description: This is a default description.
        type: parameters
      contentType:
        description: This is a default description.
        type: parameters
      fileName:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      intendedDestinations:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      targetCountry:
        description: This is a default description.
        type: parameters
  DatafeedFetchSchedule:
    properties:
      dayOfMonth:
        description: This is a default description.
        type: parameters
      fetchUrl:
        description: This is a default description.
        type: parameters
      hour:
        description: This is a default description.
        type: parameters
      minuteOfHour:
        description: This is a default description.
        type: parameters
      password:
        description: This is a default description.
        type: parameters
      timeZone:
        description: This is a default description.
        type: parameters
      username:
        description: This is a default description.
        type: parameters
      weekday:
        description: This is a default description.
        type: parameters
  DatafeedFormat:
    properties:
      columnDelimiter:
        description: This is a default description.
        type: parameters
      fileEncoding:
        description: This is a default description.
        type: parameters
      quotingMode:
        description: This is a default description.
        type: parameters
  DatafeedStatus:
    properties:
      datafeedId:
        description: This is a default description.
        type: parameters
      errors:
        description: This is a default description.
        type: parameters
      itemsTotal:
        description: This is a default description.
        type: parameters
      itemsValid:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      lastUploadDate:
        description: This is a default description.
        type: parameters
      processingStatus:
        description: This is a default description.
        type: parameters
      warnings:
        description: This is a default description.
        type: parameters
  DatafeedStatusError:
    properties:
      code:
        description: This is a default description.
        type: parameters
      count:
        description: This is a default description.
        type: parameters
      examples:
        description: This is a default description.
        type: parameters
      message:
        description: This is a default description.
        type: parameters
  DatafeedStatusExample:
    properties:
      itemId:
        description: This is a default description.
        type: parameters
      lineNumber:
        description: This is a default description.
        type: parameters
      value:
        description: This is a default description.
        type: parameters
  DatafeedsCustomBatchRequest:
    properties:
      entries:
        description: This is a default description.
        type: parameters
  DatafeedsCustomBatchRequestEntry:
    properties:
      batchId:
        description: This is a default description.
        type: parameters
      datafeedId:
        description: This is a default description.
        type: parameters
      merchantId:
        description: This is a default description.
        type: parameters
      method:
        description: This is a default description.
        type: parameters
  DatafeedsCustomBatchResponse:
    properties:
      entries:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  DatafeedsCustomBatchResponseEntry:
    properties:
      batchId:
        description: This is a default description.
        type: parameters
  DatafeedsListResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      resources:
        description: This is a default description.
        type: parameters
  DatafeedstatusesCustomBatchRequest:
    properties:
      entries:
        description: This is a default description.
        type: parameters
  DatafeedstatusesCustomBatchRequestEntry:
    properties:
      batchId:
        description: This is a default description.
        type: parameters
      datafeedId:
        description: This is a default description.
        type: parameters
      merchantId:
        description: This is a default description.
        type: parameters
      method:
        description: This is a default description.
        type: parameters
  DatafeedstatusesCustomBatchResponse:
    properties:
      entries:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  DatafeedstatusesCustomBatchResponseEntry:
    properties:
      batchId:
        description: This is a default description.
        type: parameters
  DatafeedstatusesListResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      resources:
        description: This is a default description.
        type: parameters
  DeliveryTime:
    properties:
      maxTransitTimeInDays:
        description: This is a default description.
        type: parameters
      minTransitTimeInDays:
        description: This is a default description.
        type: parameters
  Error:
    properties:
      domain:
        description: This is a default description.
        type: parameters
      message:
        description: This is a default description.
        type: parameters
      reason:
        description: This is a default description.
        type: parameters
  Errors:
    properties:
      code:
        description: This is a default description.
        type: parameters
      errors:
        description: This is a default description.
        type: parameters
      message:
        description: This is a default description.
        type: parameters
  Headers:
    properties:
      locations:
        description: This is a default description.
        type: parameters
      numberOfItems:
        description: This is a default description.
        type: parameters
      postalCodeGroupNames:
        description: This is a default description.
        type: parameters
      prices:
        description: This is a default description.
        type: parameters
      weights:
        description: This is a default description.
        type: parameters
  Installment:
    properties:
      months:
        description: This is a default description.
        type: parameters
  Inventory:
    properties:
      availability:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      quantity:
        description: This is a default description.
        type: parameters
      salePriceEffectiveDate:
        description: This is a default description.
        type: parameters
      sellOnGoogleQuantity:
        description: This is a default description.
        type: parameters
  InventoryCustomBatchRequest:
    properties:
      entries:
        description: This is a default description.
        type: parameters
  InventoryCustomBatchRequestEntry:
    properties:
      batchId:
        description: This is a default description.
        type: parameters
      merchantId:
        description: This is a default description.
        type: parameters
      productId:
        description: This is a default description.
        type: parameters
      storeCode:
        description: This is a default description.
        type: parameters
  InventoryCustomBatchResponse:
    properties:
      entries:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  InventoryCustomBatchResponseEntry:
    properties:
      batchId:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  InventoryPickup:
    properties:
      pickupMethod:
        description: This is a default description.
        type: parameters
      pickupSla:
        description: This is a default description.
        type: parameters
  InventorySetRequest:
    properties:
      availability:
        description: This is a default description.
        type: parameters
      quantity:
        description: This is a default description.
        type: parameters
      salePriceEffectiveDate:
        description: This is a default description.
        type: parameters
      sellOnGoogleQuantity:
        description: This is a default description.
        type: parameters
  InventorySetResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
  LocationIdSet:
    properties:
      locationIds:
        description: This is a default description.
        type: parameters
  LoyaltyPoints:
    properties:
      name:
        description: This is a default description.
        type: parameters
      pointsValue:
        description: This is a default description.
        type: parameters
      ratio:
        description: This is a default description.
        type: parameters
  Order:
    properties:
      acknowledged:
        description: This is a default description.
        type: parameters
      channelType:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      lineItems:
        description: This is a default description.
        type: parameters
      merchantId:
        description: This is a default description.
        type: parameters
      merchantOrderId:
        description: This is a default description.
        type: parameters
      paymentStatus:
        description: This is a default description.
        type: parameters
      placedDate:
        description: This is a default description.
        type: parameters
      promotions:
        description: This is a default description.
        type: parameters
  OrderAddress:
    properties:
      country:
        description: This is a default description.
        type: parameters
      fullAddress:
        description: This is a default description.
        type: parameters
      isPostOfficeBox:
        description: This is a default description.
        type: parameters
      locality:
        description: This is a default description.
        type: parameters
      postalCode:
        description: This is a default description.
        type: parameters
      recipientName:
        description: This is a default description.
        type: parameters
      region:
        description: This is a default description.
        type: parameters
      streetAddress:
        description: This is a default description.
        type: parameters
  OrderCancellation:
    properties:
      actor:
        description: This is a default description.
        type: parameters
      creationDate:
        description: This is a default description.
        type: parameters
      quantity:
        description: This is a default description.
        type: parameters
      reason:
        description: This is a default description.
        type: parameters
      reasonText:
        description: This is a default description.
        type: parameters
  OrderCustomer:
    properties:
      email:
        description: This is a default description.
        type: parameters
      explicitMarketingPreference:
        description: This is a default description.
        type: parameters
      fullName:
        description: This is a default description.
        type: parameters
  OrderDeliveryDetails:
    properties:
      phoneNumber:
        description: This is a default description.
        type: parameters
  OrderLineItem:
    properties:
      cancellations:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      quantityCanceled:
        description: This is a default description.
        type: parameters
      quantityDelivered:
        description: This is a default description.
        type: parameters
      quantityOrdered:
        description: This is a default description.
        type: parameters
      quantityPending:
        description: This is a default description.
        type: parameters
      quantityReturned:
        description: This is a default description.
        type: parameters
      quantityShipped:
        description: This is a default description.
        type: parameters
      returns:
        description: This is a default description.
        type: parameters
  OrderLineItemProduct:
    properties:
      brand:
        description: This is a default description.
        type: parameters
      channel:
        description: This is a default description.
        type: parameters
      condition:
        description: This is a default description.
        type: parameters
      contentLanguage:
        description: This is a default description.
        type: parameters
      gtin:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      imageLink:
        description: This is a default description.
        type: parameters
      itemGroupId:
        description: This is a default description.
        type: parameters
      mpn:
        description: This is a default description.
        type: parameters
      offerId:
        description: This is a default description.
        type: parameters
  OrderLineItemProductVariantAttribute:
    properties:
      dimension:
        description: This is a default description.
        type: parameters
      value:
        description: This is a default description.
        type: parameters
  OrderLineItemReturnInfo:
    properties:
      daysToReturn:
        description: This is a default description.
        type: parameters
      isReturnable:
        description: This is a default description.
        type: parameters
      policyUrl:
        description: This is a default description.
        type: parameters
  OrderLineItemShippingDetails:
    properties:
      deliverByDate:
        description: This is a default description.
        type: parameters
      shipByDate:
        description: This is a default description.
        type: parameters
  OrderLineItemShippingDetailsMethod:
    properties:
      carrier:
        description: This is a default description.
        type: parameters
      maxDaysInTransit:
        description: This is a default description.
        type: parameters
      methodName:
        description: This is a default description.
        type: parameters
      minDaysInTransit:
        description: This is a default description.
        type: parameters
  OrderPaymentMethod:
    properties:
      expirationMonth:
        description: This is a default description.
        type: parameters
      expirationYear:
        description: This is a default description.
        type: parameters
      lastFourDigits:
        description: This is a default description.
        type: parameters
      phoneNumber:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  OrderPromotion:
    properties:
      benefits:
        description: This is a default description.
        type: parameters
      effectiveDates:
        description: This is a default description.
        type: parameters
      genericRedemptionCode:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      longTitle:
        description: This is a default description.
        type: parameters
      productApplicability:
        description: This is a default description.
        type: parameters
      redemptionChannel:
        description: This is a default description.
        type: parameters
  OrderPromotionBenefit:
    properties:
      offerIds:
        description: This is a default description.
        type: parameters
      subType:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  OrderRefund:
    properties:
      actor:
        description: This is a default description.
        type: parameters
      creationDate:
        description: This is a default description.
        type: parameters
      reason:
        description: This is a default description.
        type: parameters
      reasonText:
        description: This is a default description.
        type: parameters
  OrderReturn:
    properties:
      actor:
        description: This is a default description.
        type: parameters
      creationDate:
        description: This is a default description.
        type: parameters
      quantity:
        description: This is a default description.
        type: parameters
      reason:
        description: This is a default description.
        type: parameters
      reasonText:
        description: This is a default description.
        type: parameters
  OrderShipment:
    properties:
      carrier:
        description: This is a default description.
        type: parameters
      creationDate:
        description: This is a default description.
        type: parameters
      deliveryDate:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      lineItems:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
      trackingId:
        description: This is a default description.
        type: parameters
  OrderShipmentLineItemShipment:
    properties:
      lineItemId:
        description: This is a default description.
        type: parameters
      quantity:
        description: This is a default description.
        type: parameters
  OrdersAcknowledgeRequest:
    properties:
      operationId:
        description: This is a default description.
        type: parameters
  OrdersAcknowledgeResponse:
    properties:
      executionStatus:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  OrdersAdvanceTestOrderResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
  OrdersCancelLineItemRequest:
    properties:
      lineItemId:
        description: This is a default description.
        type: parameters
      operationId:
        description: This is a default description.
        type: parameters
      quantity:
        description: This is a default description.
        type: parameters
      reason:
        description: This is a default description.
        type: parameters
      reasonText:
        description: This is a default description.
        type: parameters
  OrdersCancelLineItemResponse:
    properties:
      executionStatus:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  OrdersCancelRequest:
    properties:
      operationId:
        description: This is a default description.
        type: parameters
      reason:
        description: This is a default description.
        type: parameters
      reasonText:
        description: This is a default description.
        type: parameters
  OrdersCancelResponse:
    properties:
      executionStatus:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  OrdersCreateTestOrderRequest:
    properties:
      templateName:
        description: This is a default description.
        type: parameters
  OrdersCreateTestOrderResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      orderId:
        description: This is a default description.
        type: parameters
  OrdersCustomBatchRequest:
    properties:
      entries:
        description: This is a default description.
        type: parameters
  OrdersCustomBatchRequestEntry:
    properties:
      batchId:
        description: This is a default description.
        type: parameters
      merchantId:
        description: This is a default description.
        type: parameters
      merchantOrderId:
        description: This is a default description.
        type: parameters
      method:
        description: This is a default description.
        type: parameters
      operationId:
        description: This is a default description.
        type: parameters
      orderId:
        description: This is a default description.
        type: parameters
  OrdersCustomBatchRequestEntryCancel:
    properties:
      reason:
        description: This is a default description.
        type: parameters
      reasonText:
        description: This is a default description.
        type: parameters
  OrdersCustomBatchRequestEntryCancelLineItem:
    properties:
      lineItemId:
        description: This is a default description.
        type: parameters
      quantity:
        description: This is a default description.
        type: parameters
      reason:
        description: This is a default description.
        type: parameters
      reasonText:
        description: This is a default description.
        type: parameters
  OrdersCustomBatchRequestEntryRefund:
    properties:
      reason:
        description: This is a default description.
        type: parameters
      reasonText:
        description: This is a default description.
        type: parameters
  OrdersCustomBatchRequestEntryReturnLineItem:
    properties:
      lineItemId:
        description: This is a default description.
        type: parameters
      quantity:
        description: This is a default description.
        type: parameters
      reason:
        description: This is a default description.
        type: parameters
      reasonText:
        description: This is a default description.
        type: parameters
  OrdersCustomBatchRequestEntryShipLineItems:
    properties:
      carrier:
        description: This is a default description.
        type: parameters
      lineItems:
        description: This is a default description.
        type: parameters
      shipmentId:
        description: This is a default description.
        type: parameters
      trackingId:
        description: This is a default description.
        type: parameters
  OrdersCustomBatchRequestEntryUpdateShipment:
    properties:
      carrier:
        description: This is a default description.
        type: parameters
      shipmentId:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
      trackingId:
        description: This is a default description.
        type: parameters
  OrdersCustomBatchResponse:
    properties:
      entries:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  OrdersCustomBatchResponseEntry:
    properties:
      batchId:
        description: This is a default description.
        type: parameters
      executionStatus:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  OrdersGetByMerchantOrderIdResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
  OrdersGetTestOrderTemplateResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
  OrdersListResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      resources:
        description: This is a default description.
        type: parameters
  OrdersRefundRequest:
    properties:
      operationId:
        description: This is a default description.
        type: parameters
      reason:
        description: This is a default description.
        type: parameters
      reasonText:
        description: This is a default description.
        type: parameters
  OrdersRefundResponse:
    properties:
      executionStatus:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  OrdersReturnLineItemRequest:
    properties:
      lineItemId:
        description: This is a default description.
        type: parameters
      operationId:
        description: This is a default description.
        type: parameters
      quantity:
        description: This is a default description.
        type: parameters
      reason:
        description: This is a default description.
        type: parameters
      reasonText:
        description: This is a default description.
        type: parameters
  OrdersReturnLineItemResponse:
    properties:
      executionStatus:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  OrdersShipLineItemsRequest:
    properties:
      carrier:
        description: This is a default description.
        type: parameters
      lineItems:
        description: This is a default description.
        type: parameters
      operationId:
        description: This is a default description.
        type: parameters
      shipmentId:
        description: This is a default description.
        type: parameters
      trackingId:
        description: This is a default description.
        type: parameters
  OrdersShipLineItemsResponse:
    properties:
      executionStatus:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  OrdersUpdateMerchantOrderIdRequest:
    properties:
      merchantOrderId:
        description: This is a default description.
        type: parameters
      operationId:
        description: This is a default description.
        type: parameters
  OrdersUpdateMerchantOrderIdResponse:
    properties:
      executionStatus:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  OrdersUpdateShipmentRequest:
    properties:
      carrier:
        description: This is a default description.
        type: parameters
      operationId:
        description: This is a default description.
        type: parameters
      shipmentId:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
      trackingId:
        description: This is a default description.
        type: parameters
  OrdersUpdateShipmentResponse:
    properties:
      executionStatus:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  PostalCodeGroup:
    properties:
      country:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      postalCodeRanges:
        description: This is a default description.
        type: parameters
  PostalCodeRange:
    properties:
      postalCodeRangeBegin:
        description: This is a default description.
        type: parameters
      postalCodeRangeEnd:
        description: This is a default description.
        type: parameters
  Price:
    properties:
      currency:
        description: This is a default description.
        type: parameters
      value:
        description: This is a default description.
        type: parameters
  Product:
    properties:
      additionalImageLinks:
        description: This is a default description.
        type: parameters
      additionalProductTypes:
        description: This is a default description.
        type: parameters
      adult:
        description: This is a default description.
        type: parameters
      adwordsGrouping:
        description: This is a default description.
        type: parameters
      adwordsLabels:
        description: This is a default description.
        type: parameters
      adwordsRedirect:
        description: This is a default description.
        type: parameters
      ageGroup:
        description: This is a default description.
        type: parameters
      aspects:
        description: This is a default description.
        type: parameters
      availability:
        description: This is a default description.
        type: parameters
      availabilityDate:
        description: This is a default description.
        type: parameters
  ProductAspect:
    properties:
      aspectName:
        description: This is a default description.
        type: parameters
      destinationName:
        description: This is a default description.
        type: parameters
      intention:
        description: This is a default description.
        type: parameters
  ProductCustomAttribute:
    properties:
      name:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
      unit:
        description: This is a default description.
        type: parameters
      value:
        description: This is a default description.
        type: parameters
  ProductCustomGroup:
    properties:
      attributes:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
  ProductDestination:
    properties:
      destinationName:
        description: This is a default description.
        type: parameters
      intention:
        description: This is a default description.
        type: parameters
  ProductShipping:
    properties:
      country:
        description: This is a default description.
        type: parameters
      locationGroupName:
        description: This is a default description.
        type: parameters
      locationId:
        description: This is a default description.
        type: parameters
      postalCode:
        description: This is a default description.
        type: parameters
      region:
        description: This is a default description.
        type: parameters
      service:
        description: This is a default description.
        type: parameters
  ProductShippingDimension:
    properties:
      unit:
        description: This is a default description.
        type: parameters
      value:
        description: This is a default description.
        type: parameters
  ProductShippingWeight:
    properties:
      unit:
        description: This is a default description.
        type: parameters
      value:
        description: This is a default description.
        type: parameters
  ProductStatus:
    properties:
      creationDate:
        description: This is a default description.
        type: parameters
      dataQualityIssues:
        description: This is a default description.
        type: parameters
      destinationStatuses:
        description: This is a default description.
        type: parameters
      googleExpirationDate:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      lastUpdateDate:
        description: This is a default description.
        type: parameters
      link:
        description: This is a default description.
        type: parameters
      productId:
        description: This is a default description.
        type: parameters
      title:
        description: This is a default description.
        type: parameters
  ProductStatusDataQualityIssue:
    properties:
      detail:
        description: This is a default description.
        type: parameters
      fetchStatus:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      location:
        description: This is a default description.
        type: parameters
      severity:
        description: This is a default description.
        type: parameters
      timestamp:
        description: This is a default description.
        type: parameters
      valueOnLandingPage:
        description: This is a default description.
        type: parameters
      valueProvided:
        description: This is a default description.
        type: parameters
  ProductStatusDestinationStatus:
    properties:
      approvalStatus:
        description: This is a default description.
        type: parameters
      destination:
        description: This is a default description.
        type: parameters
      intention:
        description: This is a default description.
        type: parameters
  ProductTax:
    properties:
      country:
        description: This is a default description.
        type: parameters
      locationId:
        description: This is a default description.
        type: parameters
      postalCode:
        description: This is a default description.
        type: parameters
      rate:
        description: This is a default description.
        type: parameters
      region:
        description: This is a default description.
        type: parameters
      taxShip:
        description: This is a default description.
        type: parameters
  ProductUnitPricingBaseMeasure:
    properties:
      unit:
        description: This is a default description.
        type: parameters
      value:
        description: This is a default description.
        type: parameters
  ProductUnitPricingMeasure:
    properties:
      unit:
        description: This is a default description.
        type: parameters
      value:
        description: This is a default description.
        type: parameters
  ProductsCustomBatchRequest:
    properties:
      entries:
        description: This is a default description.
        type: parameters
  ProductsCustomBatchRequestEntry:
    properties:
      batchId:
        description: This is a default description.
        type: parameters
      merchantId:
        description: This is a default description.
        type: parameters
      method:
        description: This is a default description.
        type: parameters
      productId:
        description: This is a default description.
        type: parameters
  ProductsCustomBatchResponse:
    properties:
      entries:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  ProductsCustomBatchResponseEntry:
    properties:
      batchId:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  ProductsListResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      resources:
        description: This is a default description.
        type: parameters
  ProductstatusesCustomBatchRequest:
    properties:
      entries:
        description: This is a default description.
        type: parameters
  ProductstatusesCustomBatchRequestEntry:
    properties:
      batchId:
        description: This is a default description.
        type: parameters
      merchantId:
        description: This is a default description.
        type: parameters
      method:
        description: This is a default description.
        type: parameters
      productId:
        description: This is a default description.
        type: parameters
  ProductstatusesCustomBatchResponse:
    properties:
      entries:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  ProductstatusesCustomBatchResponseEntry:
    properties:
      batchId:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  ProductstatusesListResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      resources:
        description: This is a default description.
        type: parameters
  RateGroup:
    properties:
      applicableShippingLabels:
        description: This is a default description.
        type: parameters
      carrierRates:
        description: This is a default description.
        type: parameters
      subtables:
        description: This is a default description.
        type: parameters
  Row:
    properties:
      cells:
        description: This is a default description.
        type: parameters
  Service:
    properties:
      active:
        description: This is a default description.
        type: parameters
      currency:
        description: This is a default description.
        type: parameters
      deliveryCountry:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      rateGroups:
        description: This is a default description.
        type: parameters
  ShippingSettings:
    properties:
      accountId:
        description: This is a default description.
        type: parameters
      postalCodeGroups:
        description: This is a default description.
        type: parameters
      services:
        description: This is a default description.
        type: parameters
  ShippingsettingsCustomBatchRequest:
    properties:
      entries:
        description: This is a default description.
        type: parameters
  ShippingsettingsCustomBatchRequestEntry:
    properties:
      accountId:
        description: This is a default description.
        type: parameters
      batchId:
        description: This is a default description.
        type: parameters
      merchantId:
        description: This is a default description.
        type: parameters
      method:
        description: This is a default description.
        type: parameters
  ShippingsettingsCustomBatchResponse:
    properties:
      entries:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  ShippingsettingsCustomBatchResponseEntry:
    properties:
      batchId:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  ShippingsettingsGetSupportedCarriersResponse:
    properties:
      carriers:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  ShippingsettingsListResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      resources:
        description: This is a default description.
        type: parameters
  Table:
    properties:
      name:
        description: This is a default description.
        type: parameters
      rows:
        description: This is a default description.
        type: parameters
  TestOrder:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      lineItems:
        description: This is a default description.
        type: parameters
      predefinedDeliveryAddress:
        description: This is a default description.
        type: parameters
      promotions:
        description: This is a default description.
        type: parameters
      shippingOption:
        description: This is a default description.
        type: parameters
  TestOrderCustomer:
    properties:
      email:
        description: This is a default description.
        type: parameters
      explicitMarketingPreference:
        description: This is a default description.
        type: parameters
      fullName:
        description: This is a default description.
        type: parameters
  TestOrderLineItem:
    properties:
      quantityOrdered:
        description: This is a default description.
        type: parameters
  TestOrderLineItemProduct:
    properties:
      brand:
        description: This is a default description.
        type: parameters
      channel:
        description: This is a default description.
        type: parameters
      condition:
        description: This is a default description.
        type: parameters
      contentLanguage:
        description: This is a default description.
        type: parameters
      gtin:
        description: This is a default description.
        type: parameters
      imageLink:
        description: This is a default description.
        type: parameters
      itemGroupId:
        description: This is a default description.
        type: parameters
      mpn:
        description: This is a default description.
        type: parameters
      offerId:
        description: This is a default description.
        type: parameters
      targetCountry:
        description: This is a default description.
        type: parameters
  TestOrderPaymentMethod:
    properties:
      expirationMonth:
        description: This is a default description.
        type: parameters
      expirationYear:
        description: This is a default description.
        type: parameters
      lastFourDigits:
        description: This is a default description.
        type: parameters
      predefinedBillingAddress:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  Value:
    properties:
      carrierRateName:
        description: This is a default description.
        type: parameters
      noShipping:
        description: This is a default description.
        type: parameters
      pricePercentage:
        description: This is a default description.
        type: parameters
      subtableName:
        description: This is a default description.
        type: parameters
  Weight:
    properties:
      unit:
        description: This is a default description.
        type: parameters
      value:
        description: This is a default description.
        type: parameters
x-collection-name: Google Content API for Shopping
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