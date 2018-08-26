{
  "info": {
    "name": "Codefresh Get Progress",
    "_postman_id": "f2d5650e-6113-490d-ab2c-0bd871469af6",
    "description": "Get progress.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "3327c634-30ee-485b-a4d1-2ba9c147e1d9",
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
              "id": "967f7db2-f007-42ac-b00f-11b8a420e076"
            }
          ]
        },
        {
          "id": "bb97fa73-63cd-450f-bc0e-ad6422d1cf71",
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
              "id": "c98a6663-5fdb-439b-a559-b84f9242fbfa"
            }
          ]
        }
      ]
    },
    {
      "name": "Progress",
      "item": [
        {
          "id": "0aad34a9-8f79-4c23-b64f-7ca40652aa9b",
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
              "id": "152d0c90-1c4e-4f1b-aa81-e8b75f3718cf"
            }
          ]
        }
      ]
    }
  ]
}