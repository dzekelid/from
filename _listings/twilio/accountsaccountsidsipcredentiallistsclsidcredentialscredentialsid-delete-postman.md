{
  "info": {
    "name": "Twilio Delete SIP Credential From List",
    "_postman_id": "5566758e-f86f-4474-ac10-d8a5c8d8a2e4",
    "description": "Remove a Credential from a CredentialList.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "sip credential lists",
      "item": [
        {
          "id": "03136891-28dd-4f5a-948e-b7b7aad9dd6b",
          "name": "remove-a-credential-from-a-credentiallist",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/SIP/CredentialLists/:CLSid/Credentials/:CredentialSid"
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "CLSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "CredentialSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a Credential from a CredentialList"
          },
          "response": [
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "[\r\n  {\r\n    \"uri\": \"uri\",\r\n    \"firstpageuri\": \"firstpageuri\",\r\n    \"nextpageuri\": \"nextpageuri\",\r\n    \"previouspageuri\": \"previouspageuri\",\r\n    \"page\": \"page\",\r\n    \"pagesize\": \"pagesize\",\r\n    \"credentials\": {}\r\n  }\r\n]",
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "ef5a3041-b90b-4edc-b6f5-b55b6f742056"
            }
          ]
        }
      ]
    }
  ]
}