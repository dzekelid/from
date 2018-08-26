{
  "info": {
    "name": "Plentymarkets Delete files from the inbox",
    "_postman_id": "72062684-dd58-4c0a-9c48-07aa5adb5d2c",
    "description": "Deletes a list of files from the inbox. A list of storage keys must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Single",
      "item": [
        {
          "id": "65a293a0-255a-476b-8d28-55ca99176696",
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
              "id": "4a1fec85-4682-441f-8fa3-d9944c2f4e16"
            }
          ]
        }
      ]
    },
    {
      "name": "Files",
      "item": [
        {
          "id": "1b3370a6-5c61-4f04-a659-d9f9e7d7168c",
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
              "id": "bfccbab9-a50f-4f57-a8f3-118fee0aac83"
            }
          ]
        },
        {
          "id": "744119a9-1e0b-4f83-817e-c80e23705899",
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
              "id": "02a5e147-194f-4587-a32e-073ef756dc58"
            }
          ]
        },
        {
          "id": "91d523d7-0359-47ab-b2f3-cf7b593f19c5",
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
              "id": "9bc698fb-4ca5-4705-b05f-d5f590885d7a"
            }
          ]
        }
      ]
    },
    {
      "name": "Get",
      "item": [
        {
          "id": "71de96dc-c31b-4adf-bf0b-40dcca7f92db",
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
              "id": "7c11b4c2-5578-4c2a-a5e6-3907cbaa7843"
            }
          ]
        }
      ]
    },
    {
      "name": "Creates",
      "item": [
        {
          "id": "bc3d1d36-8af4-4429-97df-dad183155979",
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
              "id": "f47edae8-3215-4cbc-962e-7bf9712abff0"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "cd828b14-a882-43d3-8547-62aeb8b16fd1",
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
              "id": "e448c1d4-0713-4bb2-a02e-47acce6895ec"
            }
          ]
        }
      ]
    },
    {
      "name": "Remove",
      "item": [
        {
          "id": "c5092cba-9e93-40af-866d-8224083af18c",
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
              "id": "9bcc8684-c394-4903-a88e-65cc7b52cfef"
            }
          ]
        },
        {
          "id": "99c40633-c6ad-46ac-8175-20642ef66b8f",
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
              "id": "b0f79d22-70d2-4fd1-9843-700e4cea39d9"
            }
          ]
        },
        {
          "id": "f633f7db-b08f-4d38-b16c-6864bee2be2f",
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
              "id": "ab7c608f-1342-4cb3-bd5a-26d7aa4ef274"
            }
          ]
        }
      ]
    },
    {
      "name": "Unlink",
      "item": [
        {
          "id": "c53e5615-80fb-40bc-a250-8de5287c0a30",
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
              "id": "1c18e0ab-391a-4423-8718-fe5a65244907"
            }
          ]
        }
      ]
    },
    {
      "name": "Date",
      "item": [
        {
          "id": "6282b965-abda-4a8f-bb96-3c8e42da1dec",
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
              "id": "8b3f5fea-7b07-4b4e-9295-35e2ad3cb2ac"
            }
          ]
        },
        {
          "id": "a9a2f181-0d35-4646-a434-197e56ebfb30",
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
              "id": "b0f73be4-3357-4d27-aabb-8b0a2da7d658"
            }
          ]
        }
      ]
    },
    {
      "name": "Surcharge",
      "item": [
        {
          "id": "deb4f675-b950-45d4-ac46-4d08cf0f1005",
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
              "id": "cc2838ef-3b8f-4f07-83e0-711425594bff"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "912f507f-8ddc-4312-b6b6-dfdcf603d4b6",
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
              "id": "c53acb90-f75d-4987-8850-e89f7c3caf77"
            }
          ]
        }
      ]
    },
    {
      "name": "Detach",
      "item": [
        {
          "id": "25371f81-3526-445f-94e3-6f77698f4c77",
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
              "id": "116a7b48-c2f8-4b57-8e3b-c81d07520bea"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "12de3e18-bb88-44eb-8f51-c519b534de76",
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
              "id": "25cb80dd-490b-422a-bad4-48bdd2e19e0e"
            }
          ]
        },
        {
          "id": "5057f3e5-00be-4778-8438-05ed44d9f774",
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
              "id": "af7748f0-f7e2-4544-aab5-20a2b6e287b6"
            }
          ]
        }
      ]
    }
  ]
}