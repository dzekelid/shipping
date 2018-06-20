{
  "info": {
    "name": "reverb Get Shipping Provers",
    "_postman_id": "032275b4-04f4-4654-a401-0ec020fcf002",
    "description": "List of supported shipping providers",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Shipping",
      "item": [
        {
          "id": "db6d6085-c799-4fb8-bfa3-746c7d459966",
          "name": "getShippingProvers",
          "request": {
            "url": "http://api.reverb.com/api/shipping/providers",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of supported shipping providers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "173da2f2-3d26-498a-8ae9-206ce7cbd62c"
            }
          ]
        }
      ]
    }
  ]
}