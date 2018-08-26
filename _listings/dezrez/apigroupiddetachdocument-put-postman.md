{
  "info": {
    "name": "Dezrez Detaches a document from a group",
    "_postman_id": "de09b890-a67a-496b-978a-89a4ff8bbc41",
    "description": "Detaches a document from a group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Detaches",
      "item": [
        {
          "id": "92f049a5-8236-4ede-ae86-046ec386d8f0",
          "name": "Branding_DetachDocumentByidBydocumentId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/branding/:id/detachdocument"
              ],
              "query": [
                {
                  "key": "documentId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
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
            "description": "Detaches a document from a brand.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67c4d5a7-9879-44ea-917c-a9dd71c55800"
            }
          ]
        },
        {
          "id": "f7f2859a-aeb6-4a15-a637-c1c4fc5555e6",
          "name": "Group_DetachDocumentByidBydocumentId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/group/:id/detachdocument"
              ],
              "query": [
                {
                  "key": "documentId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
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
            "description": "Detaches a document from a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf317fd8-5e32-430c-bdd1-c2851d68e368"
            }
          ]
        }
      ]
    }
  ]
}