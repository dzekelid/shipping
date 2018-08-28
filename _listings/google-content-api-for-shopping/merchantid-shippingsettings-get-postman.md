{
  "info": {
    "name": "Google Content API for Shopping API Get Shipping Settings",
    "_postman_id": "ff9487fe-0d71-4841-9d11-20d37ce3bf3b",
    "description": "Lists the shipping settings of the sub-accounts in your Merchant Center account. This method can only be called for multi-client accounts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "shipping",
      "item": [
        {
          "id": "6ab2e813-7636-4b46-a95a-0375db889274",
          "name": "content.shippingsettings.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "content",
                "v2",
                ":merchantId/shippingsettings"
              ],
              "query": [
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
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
            "description": "Lists the shipping settings of the sub-accounts in your Merchant Center account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aad0d492-2935-4e35-8dbb-36d83d635844"
            }
          ]
        }
      ]
    }
  ]
}