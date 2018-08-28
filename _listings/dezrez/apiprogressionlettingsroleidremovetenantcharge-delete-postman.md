{
  "info": {
    "name": "Dezrez Remove charges from a tenant role",
    "_postman_id": "55268bf5-9136-4bac-934a-2874a7a2da0d",
    "description": "Remove charges from a tenant role.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Remove",
      "item": [
        {
          "id": "aa939bc1-5ded-4a95-aac3-942ec6842c05",
          "name": "LettingsProgression_RemoveTenantChargesByroleIdBychargeIds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/progression/lettings/:roleId/removetenantcharge"
              ],
              "query": [
                {
                  "key": "chargeIds",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "roleId",
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
            "description": "Remove charges from a tenant role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9fa174f-fde7-4ee8-b419-2f6c762b7d13"
            }
          ]
        }
      ]
    }
  ]
}