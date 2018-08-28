{
  "info": {
    "name": "Dezrez Remove a preferred company to a group",
    "_postman_id": "2a491542-20d0-4e2e-b8bf-13ef842a9c3c",
    "description": "Remove a preferred company to a group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Preferred",
      "item": [
        {
          "id": "e76c2af9-fc4a-4c9e-806f-6cf2efb34027",
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
              "id": "c4d12a00-d127-451d-bf69-610b788a7a1c"
            }
          ]
        }
      ]
    },
    {
      "name": "Remove",
      "item": [
        {
          "id": "3e9fe9ce-0111-43bc-944f-041e109d9c3a",
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
              "id": "3639c492-f17f-4da5-890e-e9c9b0a9ee7b"
            }
          ]
        }
      ]
    }
  ]
}