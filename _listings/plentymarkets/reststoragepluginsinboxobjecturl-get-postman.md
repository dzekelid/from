{
  "info": {
    "name": "Plentymarkets Get the content of a file from the inbox",
    "_postman_id": "6c06595c-2e2f-4e38-a03b-8ad85841409e",
    "description": "Gets the content of a file stored in the inbox. The storage key (i.e. file path) must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Single",
      "item": [
        {
          "id": "fdc66e91-851a-4304-9880-11e2d9cbfa7d",
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
              "id": "55c5b57c-bbf9-4ee6-ad89-72bce07c1d5c"
            }
          ]
        }
      ]
    },
    {
      "name": "Files",
      "item": [
        {
          "id": "42919df8-8ff4-4665-a1a2-d5cff7ad3870",
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
              "id": "d6a8a520-79f3-454d-9c0b-975a1f606f52"
            }
          ]
        },
        {
          "id": "23265385-df1d-4092-8f50-4dfd50add6d2",
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
              "id": "d3634bc4-daf3-4cd4-ab59-8badccabce9e"
            }
          ]
        },
        {
          "id": "5a40eec3-8d00-401b-8a6d-8f390e082a63",
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
              "id": "c1268942-3624-45f1-bb3b-1cc743ed8d6c"
            }
          ]
        }
      ]
    },
    {
      "name": "Get",
      "item": [
        {
          "id": "2fc74b61-95da-4f3b-aa3c-ca66f1e340c1",
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
              "id": "c57deadf-13c8-4994-a3ee-4face43ecb10"
            }
          ]
        }
      ]
    },
    {
      "name": "Creates",
      "item": [
        {
          "id": "980e2ed4-63bf-41ee-8db8-38193ac893cf",
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
              "id": "00ccc2b3-67bc-4924-ad7d-2667837579cc"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "cf4b1194-c069-4776-8d13-8b3c3a0582b5",
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
              "id": "497239e9-89fc-4e10-a1eb-b16132d545fc"
            }
          ]
        }
      ]
    },
    {
      "name": "Remove",
      "item": [
        {
          "id": "f3a7c497-124e-47a7-993b-ff7d07083f35",
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
              "id": "df5568b6-7fde-4f3a-88b0-8ca007970648"
            }
          ]
        },
        {
          "id": "7f222cd1-a8b9-4358-95c2-a0464b970142",
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
              "id": "2f7795ab-64d9-46ab-937c-93b0dbdc5c2e"
            }
          ]
        },
        {
          "id": "83bcb4bd-bf29-4f7f-9f5c-4a97d9ee404a",
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
              "id": "7a01e229-6a57-4691-84a4-e12b9d06ea83"
            }
          ]
        }
      ]
    },
    {
      "name": "Unlink",
      "item": [
        {
          "id": "8ce6c898-7685-41f8-a8c7-3ec5595a5a64",
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
              "id": "68deb74b-e860-4e91-aaa8-509bae0a3347"
            }
          ]
        }
      ]
    },
    {
      "name": "Date",
      "item": [
        {
          "id": "7db84925-08cc-4dd7-89fe-3ab90e5ef95c",
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
              "id": "4315a9a3-8fff-4f66-87ef-ce83b833fb1b"
            }
          ]
        },
        {
          "id": "e8a48f96-bf24-4a77-a160-855e1f2caf30",
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
              "id": "f63f61ab-bb1b-4798-9954-a7b10f08bf57"
            }
          ]
        }
      ]
    },
    {
      "name": "Surcharge",
      "item": [
        {
          "id": "b633d51e-fe66-4579-814e-309e3235a9b3",
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
              "id": "1ca163ff-0fe5-40c8-bd1d-9f870238f856"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "131fbb4c-8cdb-4844-b750-2bc1c195559a",
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
              "id": "9364aace-f94b-47bd-b96f-a93af14a9414"
            }
          ]
        }
      ]
    },
    {
      "name": "Detach",
      "item": [
        {
          "id": "1e3ef2da-fd36-4dda-bc58-c7ee0e4a621a",
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
              "id": "07ec3efb-6bfc-4f06-8fd0-bb57006a62c9"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "f169770f-194a-443e-b5fd-75937bb8ba95",
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
              "id": "3678e614-7abd-4d44-8a73-b1cd5fa6d89a"
            }
          ]
        },
        {
          "id": "b6f9f0fe-a951-405e-8cf0-b62ab37a92d5",
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
              "id": "d86d5fb8-1703-43df-931d-6a7f038404d9"
            }
          ]
        },
        {
          "id": "25c60a8e-2d1a-457d-8144-91e868ffd356",
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
              "id": "51138f17-58a4-42b3-85ef-7b40b988d738"
            }
          ]
        }
      ]
    },
    {
      "name": "Content",
      "item": [
        {
          "id": "e4185784-024e-45f5-b4c0-ed7435effbf6",
          "name": "getRestStoragePluginsInboxObjectUrl",
          "request": {
            "url": "http://example.com/rest/storage/plugins/inbox/object-url?key=%7B%7D",
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
            "description": "Gets the content of a file stored in the inbox. The storage key (i.e. file path) must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "394ea357-05c5-4ef7-8c4c-34da914859d1"
            }
          ]
        }
      ]
    }
  ]
}