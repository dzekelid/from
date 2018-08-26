{
  "info": {
    "name": "Constant Contact Get Contacts Collection from a List",
    "_postman_id": "8acf2a78-3d5a-47c2-809a-d4f237e683e6",
    "description": "Get Contacts Collection from a List",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "bbb141ab-4527-46e0-8e9d-d24deea2610c",
          "name": "list-contacts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/contacts"
              ],
              "query": [
                {
                  "key": "listid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "updatedsince",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List Contacts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9965f71-75a3-4e38-ba23-2bc3c1fc2307"
            }
          ]
        }
      ]
    },
    {
      "name": "Contacts",
      "item": [
        {
          "id": "3212a52c-3f44-4582-bd92-adbebf4f4f00",
          "name": "get-contacts-collection-from-a-list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/lists/:list-id/members"
              ],
              "variable": [
                {
                  "id": "list-id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Contacts Collection from a List"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "303b8d56-1da8-4653-8616-bf621ad9c7c0"
            }
          ]
        }
      ]
    }
  ]
}