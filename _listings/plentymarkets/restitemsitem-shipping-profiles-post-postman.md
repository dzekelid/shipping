{
  "info": {
    "name": "Plentymarkets Bulk activate shipping profiles",
    "_postman_id": "372d5cc5-792e-43eb-b19e-1807a569824c",
    "description": "Activates up to 50 shipping profiles for items",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bulk",
      "item": [
        {
          "id": "9a1841fb-23b4-47d1-a0f0-b024a75a7a54",
          "name": "postRestItemsItemShippingProfiles",
          "request": {
            "url": "http://example.com/rest/items/item_shipping_profiles",
            "method": "POST",
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
            "description": "Activates up to 50 shipping profiles for items"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c30c7f2a-fac3-47b0-9bd2-7e017339c9e1"
            }
          ]
        }
      ]
    }
  ]
}