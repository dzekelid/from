{
  "info": {
    "name": "Plentymarkets List files from the inbox",
    "_postman_id": "14dc222f-a511-409d-9278-d37ab4e471a2",
    "description": "Lists all files of all plugins stored in the inbox. A prefix can be specified to list all files of a specific\nplugin folder only.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Single",
      "item": [
        {
          "id": "f0425ff3-18c2-4ad0-ad8b-35acaa1cfa9b",
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
              "id": "9f03ed12-4ce4-465f-a29c-f15608429dea"
            }
          ]
        }
      ]
    },
    {
      "name": "Files",
      "item": [
        {
          "id": "01d99640-05dd-4557-96f2-62713f9853e7",
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
              "id": "7e918f4a-c896-4341-ad73-c208c25e4570"
            }
          ]
        },
        {
          "id": "7b9e6483-0ea2-4d03-a510-de6cdc84245f",
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
              "id": "a8cbb585-420e-4ffd-a7ed-60f6ed01a18d"
            }
          ]
        },
        {
          "id": "7dcf4d50-1366-4149-8440-a0a3f399e872",
          "name": "deleteRestStoragePluginsInbox",
          "request": {
            "url": "http://example.com/rest/storage/plugins/inbox?keyList=%7B%7D",
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
            "description": "Deletes a list of files from the inbox. A list of storage keys must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6357709-7aa2-4cee-8326-069dc0945826"
            }
          ]
        }
      ]
    },
    {
      "name": "Get",
      "item": [
        {
          "id": "79a1176a-9267-4791-99b7-f02c0ff1db66",
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
              "id": "d79333b0-5201-4ad7-aa31-85b6491ce333"
            }
          ]
        }
      ]
    },
    {
      "name": "Creates",
      "item": [
        {
          "id": "7b7073da-d538-4af5-aba1-909141b15297",
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
              "id": "7ef2eb9f-3ca1-4982-8895-fef44cd2f899"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "0c376e27-10e9-4e62-b27c-72f388e69ea1",
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
              "id": "29c8eab7-3554-45f2-81df-166460b565a7"
            }
          ]
        }
      ]
    },
    {
      "name": "Remove",
      "item": [
        {
          "id": "b53af415-4ccf-4720-98f5-ce15eca41ec5",
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
              "id": "6793062c-be32-42db-bb8e-0e67cd407bc4"
            }
          ]
        },
        {
          "id": "3bd2dd79-e1e2-46d4-903e-6f1962049798",
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
              "id": "be223ed8-7e13-4ba9-98b7-ee37bc820b4c"
            }
          ]
        },
        {
          "id": "b658001b-3947-4162-9a4b-d6f5541ad0e5",
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
              "id": "3ee2d381-9b32-4692-bc81-618ef21e228c"
            }
          ]
        }
      ]
    },
    {
      "name": "Unlink",
      "item": [
        {
          "id": "f729a603-7d44-47fd-85b9-16b52a10774f",
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
              "id": "b6c953b1-da29-4c6a-8309-4f6dfebfdd4f"
            }
          ]
        }
      ]
    },
    {
      "name": "Date",
      "item": [
        {
          "id": "fbee5f73-a6f8-4809-af63-35881ffb525d",
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
              "id": "52292c55-c643-4729-ad92-7d6aeeb92947"
            }
          ]
        },
        {
          "id": "8e2a885c-641c-408e-9199-b37161c3472b",
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
              "id": "14ea8d8c-10a0-46c5-9f8f-e60303000d6d"
            }
          ]
        }
      ]
    },
    {
      "name": "Surcharge",
      "item": [
        {
          "id": "86e25206-d576-4e66-84a9-24177a51f017",
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
              "id": "52e7fb93-dbfb-4c9c-870f-addeb1270c93"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "c213d938-8987-4def-8a16-2d62e6c9e12b",
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
              "id": "ecee1e96-4858-4c43-a310-fac17a3bd957"
            }
          ]
        }
      ]
    },
    {
      "name": "Detach",
      "item": [
        {
          "id": "e38f9565-f0af-4b59-9377-6d8fbf0cf672",
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
              "id": "8c504aae-5745-48ae-8772-2f91ccb436b4"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "ce70b126-7fb5-4137-b843-fc786e550d3c",
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
              "id": "029426db-f942-44ea-bd6e-36e9b51f56b1"
            }
          ]
        },
        {
          "id": "12ed5958-35c5-489a-9d0e-de1039db12e0",
          "name": "getRestStorageFrontendFiles",
          "request": {
            "url": "http://example.com/rest/storage/frontend/files?continuationToken=%7B%7D",
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
            "description": "List files from frontend storage. append public cloudfront url to each retrieved object.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3b74c5a-95aa-4807-847e-acc575f75917"
            }
          ]
        },
        {
          "id": "e509513e-f22f-4eb9-aa46-43a256430041",
          "name": "getRestStoragePluginsInboxList",
          "request": {
            "url": "http://example.com/rest/storage/plugins/inbox/list?prefix=%7B%7D",
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
            "description": "Lists all files of all plugins stored in the inbox. A prefix can be specified to list all files of a specific\nplugin folder only."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc20b089-af21-4d42-90ed-7f56845549c3"
            }
          ]
        }
      ]
    }
  ]
}