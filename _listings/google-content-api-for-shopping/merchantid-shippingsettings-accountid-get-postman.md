{
  "info": {
    "name": "Google Content API for Shopping API Get Shipping Settings",
    "_postman_id": "6e25a72a-1c9f-4bf0-8873-a268aa0ff1e8",
    "description": "Retrieves the shipping settings of the account. This method can only be called for accounts to which the managing account has access: either the managing account itself or sub-accounts if the managing account is a multi-client account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "shipping",
      "item": [
        {
          "id": "f2e322dc-d5e1-44f9-83f8-4496fe2f98bf",
          "name": "content.shippingsettings.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "content",
                "v2",
                ":merchantId/shippingsettings/:accountId"
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "merchantId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the shipping settings of the account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70272b2a-a590-4d1d-8013-1728c6a8cb49"
            }
          ]
        }
      ]
    }
  ]
}