{
  "info": {
    "name": "Plentymarkets Deactivate a shipping profile",
    "_postman_id": "fd3a6f80-8753-4955-91ec-84bdd980a865",
    "description": "Unlinks a shipping profile from the item. The ID of the item must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Deactivate",
      "item": [
        {
          "id": "f551bc79-a7e7-4aa7-91f2-0a95f15bdc23",
          "name": "deleteRestCategoriesClients",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/categories/:id/clients"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deactivate availability for clients."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11ce02fe-fe05-4a1f-b680-19f53f512fa0"
            }
          ]
        },
        {
          "id": "9549b5c1-b0e8-4b15-bc11-0caaec77b991",
          "name": "deleteRestItemsBarcodesBarcodeReferrerReferrer",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/barcodes/:barcodeId/referrer/:referrerId"
              ],
              "variable": [
                {
                  "id": "barcodeId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "referrerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deactivate a referrer for a barcode. The ID of the barcode and the ID of the referrer must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30dd3b1d-a457-4c49-a41c-662817dc8dd7"
            }
          ]
        },
        {
          "id": "5679ba06-2ddd-4705-830c-feda274942f9",
          "name": "deleteRestItemsSalesPricesAccountsAccounttypeAccount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/sales_prices/:id/accounts/:accountType/:accountId"
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "accountType",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deactivates a referrer account for a sales price."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25a876c2-7e1c-4d9a-930b-b005ab2db7fc"
            }
          ]
        },
        {
          "id": "f8c0dcd7-639d-4b81-ba30-9172ff93033f",
          "name": "deleteRestItemsSalesPricesCountriesCountry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/sales_prices/:id/countries/:countryId"
              ],
              "variable": [
                {
                  "id": "countryId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deactivates a country for a sales price."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aeb481a4-9c93-4e04-9a65-16ad936f6428"
            }
          ]
        },
        {
          "id": "3bf97a78-bec6-467a-a980-3a932294b08d",
          "name": "deleteRestItemsSalesPricesCurrenciesCurrency",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/sales_prices/:id/currencies/:currency"
              ],
              "variable": [
                {
                  "id": "currency",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deactivate a currency for a sales price. The ID of the sales price and the ISO code of the currency must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50567e34-bd2e-46ac-aeaa-e644cd79859a"
            }
          ]
        },
        {
          "id": "7391aad0-e220-4ccf-b378-bbf2e6cfcce2",
          "name": "deleteRestItemsSalesPricesOnlineStoresWebstore",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/sales_prices/:id/online_stores/:webstoreId"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "webstoreId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deactivates a client (store) for a sales price. The ID of the sales price and the ID of the client (store) must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f6d1eeb-9a80-481a-b3b0-d1e9f7558689"
            }
          ]
        },
        {
          "id": "806d8418-fa70-4458-914e-0c40b48b7d60",
          "name": "deleteRestItemsItemItemShippingProfiles",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:itemId/item_shipping_profiles"
              ],
              "variable": [
                {
                  "id": "itemId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deactivates all shipping profiles of an item. The ID of the item must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47a8e2b5-7580-46d2-a7e1-8175afdaed52"
            }
          ]
        },
        {
          "id": "d1ca32dc-184f-47fe-ab8c-4826597ca15e",
          "name": "deleteRestItemsItemItemShippingProfiles",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:itemId/item_shipping_profiles/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "itemId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Unlinks a shipping profile from the item. The ID of the item must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "827341dd-c53b-4a33-a520-49829fc29e58"
            }
          ]
        }
      ]
    }
  ]
}