{
  "info": {
    "name": "Codefresh Get Repos Settings Repoowner Reponame",
    "_postman_id": "20ef10f2-d4ce-4f98-ba0e-9a50b22d19f2",
    "description": "Get repos settings repoowner reponame.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "f290ce32-fef9-47b6-8c12-671d7a4be6f7",
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
              "id": "d6eb7198-8cd8-401c-8f13-4adb6afb29b2"
            }
          ]
        },
        {
          "id": "6d77e0a7-f82a-49d9-b387-9e1b06c16c96",
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
              "id": "467c4bc5-07f4-460f-bcec-81ea15834903"
            }
          ]
        }
      ]
    },
    {
      "name": "Progress",
      "item": [
        {
          "id": "93006f03-9a3e-430e-96c5-ab6d36365abc",
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
              "id": "29a18299-d1a7-480f-a5d2-d5122265eed8"
            }
          ]
        },
        {
          "id": "f504eea2-2041-4cdb-8625-31d933803b31",
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
              "id": "336991db-0c58-465b-922d-1cd87717826b"
            }
          ]
        }
      ]
    },
    {
      "name": "Repos",
      "item": [
        {
          "id": "9a084778-6430-43d3-82cc-5fc3dd1c4908",
          "name": "getReposSettingsRepoownerReponame",
          "request": {
            "url": {
              "protocol": "http",
              "host": "g.codefresh.io",
              "path": [
                "api",
                "repos/settings/:repoOwner/:repoName"
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
                  "id": "repoOwner",
                  "value": "repoOwner",
                  "type": "string"
                },
                {
                  "id": "repoName",
                  "value": "repoName",
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
            "description": "Get repos settings repoowner reponame."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "246833b9-8180-43fc-af1a-b8dd20c5aa48"
            }
          ]
        }
      ]
    }
  ]
}