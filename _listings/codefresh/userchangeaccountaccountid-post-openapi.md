---
swagger: "2.0"
x-collection-name: Codefresh
x-complete: 0
info:
  title: Codefresh Post User Changeaccount Accountid
  description: Post user changeaccount accountid.
  termsOfService: http://www.codefresh.io
  contact:
    name: Codefresh api team
    url: http://www.codefresh.io
  version: 1.0.0
host: g.codefresh.io
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user:
    get:
      summary: Get User
      description: Get user.
      operationId: getUser
      x-api-path-slug: user-get
      responses:
        200:
          description: OK
      tags:
      - User
  /user/changeaccount/{accountId}:
    post:
      summary: Post User Changeaccount Accountid
      description: Post user changeaccount accountid.
      operationId: postUserChangeaccountAccount
      x-api-path-slug: userchangeaccountaccountid-post
      parameters:
      - in: path
        name: accountId
        description: id of an object
      responses:
        200:
          description: OK
      tags:
      - User
      - Changeaccount
      - Accountid
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---