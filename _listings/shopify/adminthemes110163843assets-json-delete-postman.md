{
  "info": {
    "name": "Shopify Remove assets from your shop",
    "_postman_id": "771234d9-2805-4126-8b21-a2369ceefb07",
    "description": "Remove assets from your shop.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "5b06722e-e8d2-4ca9-b612-c5d3beebc0f7",
          "name": "getAdminThemes110163843Assets.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/themes/110163843/assets.json",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of all theme assets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21ef13ab-67fd-4f57-b8f2-fa3dc040b19a"
            }
          ]
        },
        {
          "id": "b860c7d3-742f-4490-8010-a6179d6e77b4",
          "name": "deleteAdminThemes110163843Assets.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/themes/110163843/assets.json",
            "method": "DELETE",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Remove assets from your shop."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b87cb01-d923-49c6-85e0-93633e997792"
            }
          ]
        }
      ]
    }
  ]
}