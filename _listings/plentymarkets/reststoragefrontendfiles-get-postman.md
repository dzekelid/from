{
  "info": {
    "name": "Plentymarkets List files from frontend storage. Append public cloudfront url to each retrieved object.",
    "_postman_id": "48df89f9-1aa7-4818-b1ec-4c3a2d8d072e",
    "description": "List files from frontend storage. append public cloudfront url to each retrieved object..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Single",
      "item": [
        {
          "id": "511295c2-77eb-43c3-8eb0-223f84f1f481",
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
              "id": "82db04cb-a8e2-49c0-ae15-fb86e3136682"
            }
          ]
        }
      ]
    },
    {
      "name": "Files",
      "item": [
        {
          "id": "67f57f26-456b-4312-9b35-f17d1ae0a40a",
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
              "id": "1ce6fbc0-8e52-458c-86ea-f2f92b1ccbb6"
            }
          ]
        },
        {
          "id": "8661f383-3f4a-4fd1-8a9c-40f720c38b78",
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
              "id": "206c4d29-48c0-4c65-b8bc-1879becb7150"
            }
          ]
        }
      ]
    },
    {
      "name": "Get",
      "item": [
        {
          "id": "19a8f49f-69a7-458b-8969-6d2596948f42",
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
              "id": "65f0fd7d-2337-4dcc-b6da-ea96959cd564"
            }
          ]
        }
      ]
    },
    {
      "name": "Creates",
      "item": [
        {
          "id": "6ca66293-b550-4cc6-85e5-cca57c949cba",
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
              "id": "6c8ed73f-7a92-4715-b1d7-88950d17756c"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "a3485356-c345-4607-8c17-1ffd1525a60c",
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
              "id": "d468734c-2ddd-4863-b9a0-0758fc51c9d9"
            }
          ]
        }
      ]
    },
    {
      "name": "Remove",
      "item": [
        {
          "id": "4fbc1319-c564-4c39-873d-020f88544966",
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
              "id": "e9cced63-c578-4394-acd4-afcbce7ff61b"
            }
          ]
        },
        {
          "id": "d902020a-9b87-4cf5-8718-b6e6f6509f70",
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
              "id": "a3bbedb4-e183-40fc-9ccc-1554949a4e99"
            }
          ]
        },
        {
          "id": "ae0ecb7d-d652-4fc2-93d0-27055f9745b8",
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
              "id": "a5b7e055-52de-424f-8fd2-319d3ceefb42"
            }
          ]
        }
      ]
    },
    {
      "name": "Unlink",
      "item": [
        {
          "id": "45cc302f-fb79-4bbe-b042-22dfae68cf87",
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
              "id": "49271910-20b7-49cf-84f1-0bcdc5a3efee"
            }
          ]
        }
      ]
    },
    {
      "name": "Date",
      "item": [
        {
          "id": "499083b1-6bb9-4dcd-a2b0-00f6848e306c",
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
              "id": "58eb60c7-18d6-4d21-ad54-c72ded70b464"
            }
          ]
        },
        {
          "id": "ac1e251e-b6f5-46dd-9afa-adf9e379ff7c",
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
              "id": "3a9d0fb5-53de-4343-8b90-02aecd85734a"
            }
          ]
        }
      ]
    },
    {
      "name": "Surcharge",
      "item": [
        {
          "id": "486a8b94-05b3-4fcf-8da1-d7e54fa448cc",
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
              "id": "600a5682-296b-45ea-a56c-cd28390a893c"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "027269c1-1b46-449c-affb-284c7a41c7af",
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
              "id": "6377edc6-d8b4-4ef5-bb7f-6684a2eaf06f"
            }
          ]
        }
      ]
    },
    {
      "name": "Detach",
      "item": [
        {
          "id": "bad81897-21a8-446f-9d58-a73bc2e91c8f",
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
              "id": "4aca1de7-a002-455c-b66c-7ae05535bdc1"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "50fe93bb-bda6-45dd-94b3-8bebf0653166",
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
              "id": "e7c3fd62-ab7f-456e-a793-da207612b81f"
            }
          ]
        },
        {
          "id": "b3dc7301-bf13-4a1d-956e-8bafa2e7343d",
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
              "id": "007c1f5c-eb08-4fb5-881f-74a05f558f89"
            }
          ]
        }
      ]
    }
  ]
}