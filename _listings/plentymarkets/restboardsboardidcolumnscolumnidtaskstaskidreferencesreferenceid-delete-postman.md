{
  "info": {
    "name": "Plentymarkets Deletes a reference from a given task.",
    "_postman_id": "dd232a82-5fb0-4210-bee7-d75c891535da",
    "description": "Deletes a reference from a given task..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Single",
      "item": [
        {
          "id": "96613383-35ee-4078-91db-66146f0173d6",
          "name": "getRestAccountsContactsContactDocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/contacts/:contactId/document"
              ],
              "query": [
                {
                  "key": "key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "contactId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a single storage object from contact documents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3be8903a-bc50-4986-b3be-bdf3f4d16de8"
            }
          ]
        }
      ]
    },
    {
      "name": "Files",
      "item": [
        {
          "id": "d47dded6-3667-4c07-9feb-213062f402c9",
          "name": "deleteRestAccountsContactsContactDocuments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/contacts/:contactId/documents"
              ],
              "query": [
                {
                  "key": "keyList",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "contactId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Delete files from contact documents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c97cfc0d-dddf-411c-a259-b175774fc229"
            }
          ]
        }
      ]
    },
    {
      "name": "Get",
      "item": [
        {
          "id": "7ae96d9f-14b0-47ea-b6b1-2ab337b77919",
          "name": "getRestAccountsContactsContactVcard",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/contacts/:contactId/vcard"
              ],
              "variable": [
                {
                  "id": "contactId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a filestream of vcard from customer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6689d73-6def-434a-9e3d-30093e76e0f6"
            }
          ]
        }
      ]
    },
    {
      "name": "Creates",
      "item": [
        {
          "id": "357bb43e-da28-4106-a8f3-b8118dd95698",
          "name": "postRestBoardsBoardColumnsColumnTasksTaskReferences",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/boards/:boardId/columns/:columnId/tasks/:taskId/references"
              ],
              "query": [
                {
                  "key": "referenceValue",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "boardId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "columnId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "taskId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new reference from a given task to a contact or a ticket.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c69ac09c-4d3d-4864-a109-e8e7dff5258d"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "f25bcc4b-f656-4f58-82cb-f2441f5252c9",
          "name": "deleteRestBoardsBoardColumnsColumnTasksTaskReferencesReference",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/boards/:boardId/columns/:columnId/tasks/:taskId/references/:referenceId"
              ],
              "variable": [
                {
                  "id": "boardId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "columnId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "referenceId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "taskId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a reference from a given task.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90cfa3e2-4731-41e1-8ad9-d7913b4f9df5"
            }
          ]
        }
      ]
    }
  ]
}