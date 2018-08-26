{
  "info": {
    "name": "Dezrez Remove certificate from a property",
    "_postman_id": "286b36d2-8c37-4d0c-809f-89bd652b4039",
    "description": "Remove certificate from a property.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Remove",
      "item": [
        {
          "id": "a6c70707-e566-41dd-9b6a-c19f287b51c2",
          "name": "Property_RemoveCertificateByidBycertificateId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/property/:id/certificate/remove"
              ],
              "query": [
                {
                  "key": "certificateId",
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
            "method": "DELETE",
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
            "description": "Remove certificate from a property."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebe5e55f-567a-4975-b86c-bcabec21cd6c"
            }
          ]
        }
      ]
    }
  ]
}