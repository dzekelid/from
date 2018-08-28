{
  "info": {
    "name": "Shopify Get all the events from a particular product",
    "_postman_id": "1a528cd5-f54f-4b4a-850c-b6bd935e8e48",
    "description": "Get all the events from a particular product.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "51345514-4544-4684-83c5-8af5a1d66b8d",
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
              "id": "3a76d359-6132-4f35-aebf-48aa787cdf97"
            }
          ]
        },
        {
          "id": "f10a2ab7-8178-416c-bcbc-721923f51e1c",
          "name": "getAdminProducts7990943555Events.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/products/7990943555/events.json",
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
            "description": "Get all the events from a particular product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31a7a015-aca4-49c7-ad23-d3c3ce4cabb4"
            }
          ]
        }
      ]
    }
  ]
}