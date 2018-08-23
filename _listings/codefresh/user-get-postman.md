{
  "info": {
    "name": "Codefresh Get User",
    "_postman_id": "78198792-17dc-4637-acfb-a3ce8542c281",
    "description": "Get user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "a308e7fb-197c-47c3-9fb9-cfeb4d577b2f",
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
              "id": "945e85b9-3537-4f61-a858-6f6569a32a0d"
            }
          ]
        }
      ]
    }
  ]
}