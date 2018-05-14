{
  "info": {
    "name": "Google Content API for Shopping API Get Account Shipping",
    "_postman_id": "adbc4bcc-4b78-4fe2-ab64-b02c0d208b54",
    "description": "Lists the shipping settings of the sub-accounts in your Merchant Center account. This method can only be called for multi-client accounts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "account",
      "item": [
        {
          "id": "3caabcb8-aff9-494f-9fa3-1e493a3eb002",
          "name": "content.accountshipping.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "content",
                "v2",
                ":merchantId/accountshipping"
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
              "id": "18980490-4061-426e-a9ab-8e88d3a7476d"
            }
          ]
        }
      ]
    }
  ]
}