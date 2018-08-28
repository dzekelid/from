{
  "info": {
    "name": "Dezrez Remove an individual payment from batch export",
    "_postman_id": "5fe125d3-8e4d-480f-9911-d3ee13dadeb0",
    "description": "Remove an individual payment from batch export.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Remove",
      "item": [
        {
          "id": "84296924-b7f3-437e-bed7-d9a56abfacdf",
          "name": "AccountingExport_RemoveFromBatchByidBypaymentId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/accounting/exports/batch/:id/removepayment"
              ],
              "query": [
                {
                  "key": "paymentId",
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
            "description": "Remove an individual payment from batch export."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "195eaaa1-68d7-4a1c-b8ab-15953646ee86"
            }
          ]
        }
      ]
    }
  ]
}