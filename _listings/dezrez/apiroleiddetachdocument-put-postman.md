{
  "info": {
    "name": "Dezrez Detaches a document from a role",
    "_postman_id": "505efd89-5418-46b6-bd2a-6a294222977d",
    "description": "Detaches a document from a role.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Detaches",
      "item": [
        {
          "id": "2f738d51-c9fd-4755-bf4f-9bc2f0f457ce",
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
              "id": "95106db8-7d4e-4f24-a243-b7719e81b788"
            }
          ]
        },
        {
          "id": "b66ffa51-e16f-41e6-9de7-2e39d54ed38e",
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
              "id": "0bcb42c7-d06e-4317-a111-7978d63b02ab"
            }
          ]
        },
        {
          "id": "ba09e131-58b8-4f68-8832-cd45ec8afdb3",
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
              "id": "52d52d7a-f90b-43f4-8c41-7780d914522b"
            }
          ]
        },
        {
          "id": "bd0259aa-1e79-4d00-9c92-d3ae036f08a0",
          "name": "Property_DetachDocumentByidBydocumentId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/property/:id/detachdocument"
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
            "description": "Detaches a document from a property."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "220dbdf6-94ee-4376-982a-ae78ede27c32"
            }
          ]
        },
        {
          "id": "fdf3d2f9-a24f-4e09-8156-b5e76b3cdbb9",
          "name": "Role_DetachDescriptionByidBydescriptionId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/role/:id/detachdescription"
              ],
              "query": [
                {
                  "key": "descriptionId",
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
            "description": "Detaches a description from a role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9f3b7de-5660-4840-b53e-9d94bb52033b"
            }
          ]
        },
        {
          "id": "7ec322c9-24b5-4a8c-b21a-07f25865e530",
          "name": "Role_DetachDocumentByidBydocumentId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/role/:id/detachdocument"
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
            "description": "Detaches a document from a role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d08c23f-c1e8-4bd8-bc67-a1c09777cfcc"
            }
          ]
        }
      ]
    }
  ]
}