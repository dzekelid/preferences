{
  "info": {
    "name": "Dezrez Add a preferred company to a group",
    "_postman_id": "9e64c32b-b9a0-4cf5-9c28-c808c98c6955",
    "description": "Add a preferred company to a group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Preferred",
      "item": [
        {
          "id": "e90386af-6c9e-45fc-8a75-c06fad2e274b",
          "name": "Group_AddPreferredCompanyByidBycompanyIdBypreferredContactId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/group/:id/addpreferredcompany"
              ],
              "query": [
                {
                  "key": "companyId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "preferredContactId",
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
            "method": "POST",
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
            "description": "Add a preferred company to a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f218acd-2ebb-4208-b7db-115622239d20"
            }
          ]
        }
      ]
    },
    {
      "name": "Remove",
      "item": [
        {
          "id": "eb31c4d2-ddf7-4cef-8083-5c12d4017af1",
          "name": "Group_RemovePreferredCompanyByidBycompanyId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/group/:id/removepreferredcompany"
              ],
              "query": [
                {
                  "key": "companyId",
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
            "method": "POST",
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
            "description": "Remove a preferred company to a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33615127-65a4-468b-90da-b51271f95e87"
            }
          ]
        }
      ]
    }
  ]
}