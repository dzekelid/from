{
  "info": {
    "name": "Plentymarkets Get surcharge types from module configuration",
    "_postman_id": "e6203c48-908a-4bf9-8a7d-cc1c46936683",
    "description": "Get surcharge types from module configuration.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "3451e19e-f267-43be-94af-99e4ebcaa475",
          "name": "getRestAccountingLocationsRevenueAccountConfigurations",
          "request": {
            "url": "http://example.com/rest/accounting/locations/revenue_account_configurations?itemsPerPage=%7B%7D&page=%7B%7D",
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
            "description": "Lists revenue account configurations of a system. The revenue accounts are returned as paginated result. By default 50 revenue accounts are on one page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7bc49072-33e5-4b30-baf3-85e0f2b951e2"
            }
          ]
        },
        {
          "id": "52c282e3-e5c6-43a1-b9a4-2b97cf067470",
          "name": "getRestVat",
          "request": {
            "url": "http://example.com/rest/vat?columns=%7B%7D&itemsPerPage=%7B%7D&page=%7B%7D&with=%7B%7D",
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
            "description": "Lists the VAT configurations for the given filter. Possible filters are <code>locationId</code>, <code>countryId</code>, <code>taxIdNumber</code> and <code>startedAt</code>."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb206730-5f94-4b03-8558-19c3ccb52664"
            }
          ]
        },
        {
          "id": "9dab637e-b1dc-48bd-9470-349958930514",
          "name": "getRestVatLocationsLocation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/vat/locations/:locationId"
              ],
              "query": [
                {
                  "key": "columns",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "with",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "locationId",
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
            "description": "Lists the VAT configurations for all countries of one accounting location"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e4d09f9-4298-4e41-84fe-dd75f32619ed"
            }
          ]
        }
      ]
    },
    {
      "name": "Revenue",
      "item": [
        {
          "id": "f01af3ae-3b26-4af0-9e32-f745b8fcf953",
          "name": "getRestAccountingLocationsLocationCountriesCountryRevenueAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/:locationId/countries/:countryId/revenue_accounts"
              ],
              "variable": [
                {
                  "id": "countryId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "locationId",
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
            "description": "Get the revenue account configuration of a country. The ID of the accounting location that the country is associated with as well as the ID of the country must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c13a9bd-ea30-498f-9d32-155f6e192183"
            }
          ]
        },
        {
          "id": "35e33de5-891c-47be-bc90-b7b2b0a85769",
          "name": "getRestAccountingLocationsLocationRevenueAccountConfigurations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/:locationId/revenue_account_configurations"
              ],
              "variable": [
                {
                  "id": "locationId",
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
            "description": "Gets the revenue account configuration of an accounting location. A revenue account location configuration contains several revenue accounts. The ID of the accounting location has to be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55638e95-4daa-4825-99c4-73f50791a543"
            }
          ]
        }
      ]
    },
    {
      "name": "Debtor",
      "item": [
        {
          "id": "1cb57272-4d63-4a89-80eb-e35a0aaa9f13",
          "name": "getRestAccountingLocationsLocationDebtorAccountConfigurations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/:locationId/debtor_account_configurations"
              ],
              "variable": [
                {
                  "id": "locationId",
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
            "description": "Gets the debtor account configuration of an accounting location. The ID of the accounting location has to be specified. The debtor account configuration can contain one standard debtor account only or e.g. several accounts for each country of delivery."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "519735a9-f88f-4317-86d3-ca662dfa8b62"
            }
          ]
        }
      ]
    },
    {
      "name": "Posting",
      "item": [
        {
          "id": "5ff149cd-bd7c-424c-8b42-28c800b9bc5d",
          "name": "getRestAccountingLocationsLocationAddingKeyConfigurations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/:locationId/posting_key_configurations"
              ],
              "variable": [
                {
                  "id": "locationId",
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
            "description": "Gets a posting key configuration of an accounting location. The ID of the accounting location has to be specified. The posting key configuration can contain up to 4 posting keys."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d991d415-6967-4639-aad5-7d5865e71cd8"
            }
          ]
        }
      ]
    },
    {
      "name": "Item",
      "item": [
        {
          "id": "5a5cc95f-6e53-4592-ac70-a7b7ef235dd5",
          "name": "getRestItemSetsSetConfig",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/item_sets/:setId/config"
              ],
              "variable": [
                {
                  "id": "setId",
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
            "description": "Get the item set configuration of an item set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd8871fb-bc07-4616-960f-cdbdd5b6043b"
            }
          ]
        },
        {
          "id": "c1d60dc4-8de6-4319-a196-4c578dc7b3be",
          "name": "putRestItemSetsSetConfig",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/item_sets/:setId/config"
              ],
              "variable": [
                {
                  "id": "setId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
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
            "description": "Update an item set configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a3933d7-7a42-4d99-82a4-b36dfbef6dd9"
            }
          ]
        }
      ]
    },
    {
      "name": "Surcharge",
      "item": [
        {
          "id": "b0bab533-e3b0-4d7c-8310-66d16d5e57be",
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
              "id": "309be0fc-a80d-4c6e-a2d0-dcc7f2e0e70a"
            }
          ]
        }
      ]
    }
  ]
}