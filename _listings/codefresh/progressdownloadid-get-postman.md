{
  "info": {
    "name": "Codefresh Get Progress Download",
    "_postman_id": "11348e6a-d66a-48e7-94f8-da11410c8125",
    "description": "Get progress download.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "bf0ab5b6-bc42-458a-8dd6-6f2bf2432ccb",
          "name": "getUser",
          "request": {
            "url": "http://g.codefresh.io/api/user",
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
            "description": "Get user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "650217a8-2077-4872-8049-7f53576db33a"
            }
          ]
        },
        {
          "id": "b41c39ab-7261-4a92-a45c-6661b84e0746",
          "name": "postUserChangeaccountAccount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "g.codefresh.io",
              "path": [
                "api",
                "user/changeaccount/:accountId"
              ],
              "variable": [
                {
                  "id": "accountId",
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
            "description": "Post user changeaccount accountid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23588be3-45b8-491a-8a18-08f06f042935"
            }
          ]
        }
      ]
    },
    {
      "name": "Progress",
      "item": [
        {
          "id": "2704b36f-1421-49d5-99d8-d8b9b6f67d85",
          "name": "getProgress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "g.codefresh.io",
              "path": [
                "api",
                "progress/:id"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
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
            "description": "Get progress."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ddb9b9d-1986-46cc-ad99-a16e4750ed3c"
            }
          ]
        },
        {
          "id": "075e81d9-c766-4595-80a3-7ebec71eab58",
          "name": "getProgressDownload",
          "request": {
            "url": {
              "protocol": "http",
              "host": "g.codefresh.io",
              "path": [
                "api",
                "progress/download/:id"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
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
            "description": "Get progress download."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7a5db25-9e7b-47ad-a67a-7068ee35e6d7"
            }
          ]
        }
      ]
    }
  ]
}