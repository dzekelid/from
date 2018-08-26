{
  "info": {
    "name": "IBM Financial Crimes Insight for Insurance API Retrieve a specific physical object data from the database, based on its internal id",
    "_postman_id": "30ee9d87-5860-4a73-bc54-c90d15f91cf4",
    "description": "This method is used to retrieve specific physical object data from the database, based on its internal id",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Retrieve",
      "item": [
        {
          "id": "dce0393c-6e13-4ceb-93b7-218f34079032",
          "name": "getPhysicalObject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "fcihost.ibm.com",
              "path": [
                "ibm/fci/platform/fact/physical_object/:id"
              ],
              "port": "9443",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "IBM-FCI-Role",
                "value": "{}",
                "description": "Userid / password for user with appropriate role",
                "disabled": false
              },
              {
                "key": "IBM-FCI-Token",
                "value": "{}",
                "description": "Security token obtained for execution",
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
            "description": "This method is used to retrieve specific physical object data from the database, based on its internal id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ee3b6a4-3546-49f5-bdf1-cca008cdcbeb"
            }
          ]
        },
        {
          "id": "910851aa-d4fb-4a55-bc3a-615dcba23abe",
          "name": "getWatchlistById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "fcihost.ibm.com",
              "path": [
                "ibm/fci/platform/fact/watchlist/:id"
              ],
              "port": "9443",
              "query": [
                {
                  "key": "summary",
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
            "method": "GET",
            "header": [
              {
                "key": "IBM-FCI-Role",
                "value": "{}",
                "description": "Userid / password for user with appropriate role",
                "disabled": false
              },
              {
                "key": "IBM-FCI-Token",
                "value": "{}",
                "description": "Security token obtained for execution",
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
            "description": "This method is used to retrieve the contents of a watchlist from the database"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb2e9f4a-1ebc-4bf1-ae9b-dc38e8b9cedd"
            }
          ]
        }
      ]
    }
  ]
}