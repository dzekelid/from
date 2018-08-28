{
  "info": {
    "name": "Shopify Get all the events from a particular order",
    "_postman_id": "d1ace9f6-c1a0-4d36-a787-9837337ce6fb",
    "description": "Get all the events from a particular order.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "396a24b6-cd36-4d34-b8cf-0822e8deedab",
          "name": "getAdminOrders4554953422Events.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/orders/4554953422/events.json",
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
            "description": "Get all the events from a particular order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "391013ec-108d-4fd4-9e35-7cd24d85ea50"
            }
          ]
        }
      ]
    }
  ]
}