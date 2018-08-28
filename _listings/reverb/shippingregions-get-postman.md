{
  "info": {
    "name": "reverb Get Shipping Regions",
    "_postman_id": "69cd91d6-5c6d-4c71-abb6-b66ede189d7d",
    "description": "Get shipping regions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Shipping",
      "item": [
        {
          "id": "d4cacda3-093d-492a-9503-9d2ee9516c9d",
          "name": "getShippingRegions",
          "request": {
            "url": "http://api.reverb.com/api/shipping/regions",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shipping regions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2bb8f76-1a1e-4979-82b9-14bc70488dca"
            }
          ]
        }
      ]
    }
  ]
}