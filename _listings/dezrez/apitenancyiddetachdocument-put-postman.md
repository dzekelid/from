{
  "info": {
    "name": "Dezrez Detaches a document from a tenancy role",
    "_postman_id": "0e1beb0f-08da-4cc8-a89c-7a0a9f3e3fb6",
    "description": "Detaches a document from a tenancy role.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Detaches",
      "item": [
        {
          "id": "38ead530-e5fc-41c4-955a-457c561bcc6f",
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
              "id": "df30ea86-0166-49e3-a8a3-168575ebc485"
            }
          ]
        },
        {
          "id": "406818ce-4d64-4da8-a630-dc64168ee746",
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
              "id": "20fcaa8e-2b26-473d-ac9c-a17b9d36211e"
            }
          ]
        },
        {
          "id": "d51741be-e337-49b0-ba33-d8b0ce300994",
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
              "id": "fb9ea5e8-c07d-433d-b168-e504273d3058"
            }
          ]
        },
        {
          "id": "4d3a7320-3c1a-4196-ba98-1ff93eecb314",
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
              "id": "a769ca96-4fdc-40d9-b81d-a98f418f5c29"
            }
          ]
        },
        {
          "id": "86c62024-8130-443c-b79d-da21b1dfb599",
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
              "id": "f85519d3-27ef-46b3-88bb-490782c5da8d"
            }
          ]
        },
        {
          "id": "73f9d25c-e2e3-4402-9ce4-8abfb0b39ff2",
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
              "id": "3edd1cfc-7d17-4d69-86a8-78a0db66cd11"
            }
          ]
        },
        {
          "id": "197666ef-04e2-4388-a49c-b1cad4d844a7",
          "name": "RoomDescription_DetachDocumentFromRoomByidBydocumentIdByroomId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/roomdescription/:id/detachdocumentfromroom"
              ],
              "query": [
                {
                  "key": "documentId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "roomId",
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
            "description": "Detaches a document from a room description room.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80451e29-6f49-47b4-a983-f18ea79bbb6b"
            }
          ]
        },
        {
          "id": "d616e9c6-b60f-4b2b-a39f-68b6a0e6a15a",
          "name": "Tenancy_DetachDocumentByidBydocumentId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/tenancy/:id/detachdocument"
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
            "description": "Detaches a document from a tenancy role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c015bdf-a3cd-417d-9c30-b17208dae29a"
            }
          ]
        }
      ]
    }
  ]
}