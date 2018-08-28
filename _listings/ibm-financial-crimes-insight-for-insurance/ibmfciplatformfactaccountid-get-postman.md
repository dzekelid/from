{
  "info": {
    "name": "IBM Financial Crimes Insight for Insurance API Retrieve account data from the database, for the id",
    "_postman_id": "577663bc-1d0d-48cd-b7cb-3c019c3c7d47",
    "description": "This method is used to retrieve account data from the database",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Insert",
      "item": [
        {
          "id": "7f0cdc8e-fc4d-4a9e-810b-34b6b9aec8d2",
          "name": "putAccount",
          "request": {
            "url": "http://fcihost.ibm.com:9443/ibm/fci/platform/fact/account",
            "method": "PUT",
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
            "description": "This method is used to insert account data into the database.  The XML schema is defined in the ACCOUNT.XSD file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20ae0745-88b4-4dbf-9052-0ab7783a1b9c"
            }
          ]
        }
      ]
    },
    {
      "name": "Retrieve",
      "item": [
        {
          "id": "417d4712-344a-4e02-9e3f-79d06aa6884a",
          "name": "getAccount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "fcihost.ibm.com",
              "path": [
                "ibm/fci/platform/fact/account/:id"
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
            "description": "This method is used to retrieve account data from the database"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "526a3896-297b-4fb9-aed7-1da94f08c3ef"
            }
          ]
        }
      ]
    }
  ]
}