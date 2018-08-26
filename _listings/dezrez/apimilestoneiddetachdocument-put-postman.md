{
  "info": {
    "name": "Dezrez Detaches a document from a milestone",
    "_postman_id": "d19d1066-2dda-435f-b1b5-382af13118d3",
    "description": "Detaches a document from a milestone.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Detaches",
      "item": [
        {
          "id": "d3925002-9183-4f44-83a5-484fe5141b3f",
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
              "id": "d5a85d27-3be8-4be6-819e-345265b73044"
            }
          ]
        },
        {
          "id": "3ba40993-ea25-462f-a07d-f73ade358d8f",
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
              "id": "ff252d7f-9d82-4cd5-9ab4-9e9021cfb1af"
            }
          ]
        },
        {
          "id": "f237367e-dca2-4302-9c4f-fc4b55403f08",
          "name": "Milestone_DetachDocumentByidBydocumentId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/milestone/:id/detachdocument"
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
            "description": "Detaches a document from a milestone."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "720febfe-5c01-45cc-95b1-b927bafc5b85"
            }
          ]
        }
      ]
    }
  ]
}