{
  "info": {
    "name": "reverb Get Shops Shop Shipping Profiles",
    "_postman_id": "d936dc5c-8e2b-4c59-a80a-6ae67d068890",
    "description": "List of shipping profiles for your shop",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Shops",
      "item": [
        {
          "id": "9e5ab522-0c5b-468a-97ae-bc7528a7b6da",
          "name": "getShopsShopShippingProfiles",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reverb.com",
              "path": [
                "api",
                "shops/:shop_id/shipping_profiles"
              ],
              "variable": [
                {
                  "id": "shop_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of shipping profiles for your shop"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6dc0c88-e377-4ea3-94b0-8ba4fe85508e"
            }
          ]
        }
      ]
    }
  ]
}