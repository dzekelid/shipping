{
  "info": {
    "name": "Plentymarkets List shipping countries",
    "_postman_id": "df2b8b7a-69cf-454e-aba3-8dadea9f494d",
    "description": "List shipping countries.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "ec29a811-8106-42cd-bc7e-933cf7c06512",
          "name": "getRestItemsSalesPricesCountries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/sales_prices/:id/countries"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
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
            "description": "Lists active countries for a sales price. The ID of the sales price must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5758bf4-92e9-41b1-80d2-005daba35050"
            }
          ]
        },
        {
          "id": "6b408b18-e4da-4b42-9a39-35e9699f6ae9",
          "name": "getRestOrdersShippingCountries",
          "request": {
            "url": "http://example.com/rest/orders/shipping/countries?active=%7B%7D&with=%7B%7D",
            "method": "GET",
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
            "description": "List shipping countries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f5ea9bd0-20a7-417c-acff-d00ec2d4d7f8"
            }
          ]
        }
      ]
    }
  ]
}