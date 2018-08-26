{
  "info": {
    "name": "Plentymarkets Delete files from frontend storage.",
    "_postman_id": "4c1b282f-7603-4bca-9e7b-725d27aa17e0",
    "description": "Deletes a list of files from frontend storage. A list of storage keys must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Single",
      "item": [
        {
          "id": "9581be34-e7eb-4830-b601-dec5fbb0059d",
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
              "id": "e22b8079-a096-491d-9ae1-4b1b781708f8"
            }
          ]
        }
      ]
    },
    {
      "name": "Files",
      "item": [
        {
          "id": "9c9cd5bb-55fa-433b-b94a-fc2f08d6350e",
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
              "id": "3c8b0071-9aad-42a2-b81d-cfd7f3285a62"
            }
          ]
        },
        {
          "id": "437c1971-37f2-44e6-a64a-d7033f3fde49",
          "name": "deleteRestStorageFrontendFiles",
          "request": {
            "url": "http://example.com/rest/storage/frontend/files?keyList=%7B%7D",
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
            "description": "Deletes a list of files from frontend storage. A list of storage keys must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5bd8bf2-2398-415b-9377-ec0b5debd75e"
            }
          ]
        }
      ]
    },
    {
      "name": "Get",
      "item": [
        {
          "id": "9e47317b-fd56-44e1-8694-238abab97754",
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
              "id": "53c74368-882f-47c7-9f9f-670ac0e6b8a3"
            }
          ]
        }
      ]
    },
    {
      "name": "Creates",
      "item": [
        {
          "id": "5aa127a1-f15c-40e2-a06e-63d418a57927",
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
              "id": "af05fdb1-5bc8-4464-8fa8-9df057ace084"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "c8ed119a-7199-4f02-a55a-79d8d65d3a5d",
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
              "id": "1aae54ba-4312-453c-854f-9cb0bf03d218"
            }
          ]
        }
      ]
    },
    {
      "name": "Remove",
      "item": [
        {
          "id": "14298afa-3f70-4746-920d-172d1de42f4e",
          "name": "deleteRestItemsVariationsVariationVariationCategoriesCat",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_categories/:catId"
              ],
              "variable": [
                {
                  "id": "catId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationId",
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
            "description": "Deletes the link between a category and a variation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03736e46-c30a-44a4-8b4a-d7a403c9a553"
            }
          ]
        },
        {
          "id": "5541167f-bce4-4a92-9236-2652e5af0e32",
          "name": "deleteRestPluginSetsSetPluginsPlugin",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/plugin_sets/:setId/plugins/:pluginId"
              ],
              "variable": [
                {
                  "id": "pluginId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "setId",
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
            "description": "Removes a plugin from a set and deletes all plugin files. Response content will be 'true' if the deletion was successful,\n'false' if not. If no plugin set with the given id can be found or the plugin is not associated to the set, a 404 will be returned."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0be8640-0033-415b-a505-c4f928d0c36d"
            }
          ]
        },
        {
          "id": "42b692b5-f571-499c-b617-d2fb2299da33",
          "name": "deleteRestStorageFrontendFile",
          "request": {
            "url": "http://example.com/rest/storage/frontend/file?key=%7B%7D",
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
            "description": "Remove a single object from frontend storage.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d27c8553-2da5-40ef-b23c-cfdce0c5b308"
            }
          ]
        }
      ]
    },
    {
      "name": "Unlink",
      "item": [
        {
          "id": "c5e2f9ca-0d5e-4fc7-8a7f-4dc19b5668f4",
          "name": "deleteRestItemsVariationsVariationVariationClientsPlenty",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_clients/:plentyId"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "plentyId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationId",
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
            "description": "Deletes the link between a client (store) and a variation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41d0b956-2126-4e67-81d1-96139839143e"
            }
          ]
        }
      ]
    },
    {
      "name": "Date",
      "item": [
        {
          "id": "3b2139ae-c118-4645-82b6-6b824b5ab2ac",
          "name": "deleteRestOrdersItemsDates",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/items/dates/:id"
              ],
              "variable": [
                {
                  "id": "id",
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
            "description": "Deletes the date from an order item. The ID of the date must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "311d41c5-8003-48b1-985e-1e8c7d1c513a"
            }
          ]
        },
        {
          "id": "0c033274-cb5b-4469-8b3f-823f93c5da63",
          "name": "deleteRestOrdersItemsOrderitemDatesType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/items/:orderItemId/dates/:typeId"
              ],
              "variable": [
                {
                  "id": "orderItemId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "typeId",
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
            "description": "Deletest a date from an order item. The ID of the order item and the ID of the date type must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3820c135-35ae-4975-8c21-a13293aa9e4d"
            }
          ]
        }
      ]
    },
    {
      "name": "Surcharge",
      "item": [
        {
          "id": "8ea8fa89-476c-4ba0-8ade-111b71519b99",
          "name": "getRestPropertiesGroupsSurchargeTypes",
          "request": {
            "url": "http://example.com/rest/properties/groups/surcharge/types",
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
            "description": "Get surcharge types from module configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7556adf9-875a-4207-94fc-8d21afeb410e"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "c0c99dae-c2e2-4c59-ac28-129807456101",
          "name": "getRestPropertiesGroupsTypes",
          "request": {
            "url": "http://example.com/rest/properties/groups/types",
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
            "description": "Get group types from module configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "951400b1-f621-4fb5-b7a8-c6109be591dc"
            }
          ]
        }
      ]
    },
    {
      "name": "Detach",
      "item": [
        {
          "id": "2ec69546-009a-4c05-a804-4315dd204e5d",
          "name": "deleteRestPropertiesGroupsGroupPropertiesProperty",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/properties/groups/:groupId/properties/:propertyId"
              ],
              "variable": [
                {
                  "id": "groupId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "propertyId",
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
            "description": "Detaches a property from a property group. The ID of the property and the ID of the property group must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f45f17f-92e8-450b-a889-d3e39291d9a3"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "79361f93-e7c5-4d7f-b034-50dc3be735fc",
          "name": "getRestShopBuilderPages",
          "request": {
            "url": "http://example.com/rest/shop_builder/pages",
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
            "description": "List content pages from all plugins in a given plugin set.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a23bd8e-9b47-4718-a88a-0879c6f8a03e"
            }
          ]
        }
      ]
    }
  ]
}