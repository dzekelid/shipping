{
  "info": {
    "name": "Google Content API for Shopping API Get Account Shipping",
    "_postman_id": "33e72bfd-b051-4d14-8968-921104e5ba09",
    "description": "Retrieves the shipping settings of the account. This method can only be called for accounts to which the managing account has access: either the managing account itself or sub-accounts if the managing account is a multi-client account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "account",
      "item": [
        {
          "id": "47ce4fe2-ba6e-4b5c-a291-d663c0bb5088",
          "name": "content.accountshipping.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "content",
                "v2",
                ":merchantId/accountshipping/:accountId"
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
              "id": "aea4dd52-35ce-4324-a00e-401a99d6c893"
            }
          ]
        }
      ]
    }
  ]
}