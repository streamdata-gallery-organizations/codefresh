{
  "info": {
    "name": "Codefresh Post User Changeaccount Accountid",
    "_postman_id": "8716550a-7277-4c4b-a93e-403c9ff00055",
    "description": "Post user changeaccount accountid.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "7b2162eb-54f5-46c1-a622-e8e40a7efd10",
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
              "id": "6da6ab5b-2e18-4b7a-b30c-72693812c124"
            }
          ]
        },
        {
          "id": "9c34dd3b-cb76-4148-b5b1-cb2944c89e4c",
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
              "id": "63aa73e9-5709-4cc3-ad6f-c51792f2e5a0"
            }
          ]
        }
      ]
    }
  ]
}