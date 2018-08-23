---
swagger: "2.0"
x-collection-name: Codefresh
x-complete: 0
info:
  title: Codefresh Parameters Images External
  description: Parameters images external.
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
  /progress/{id}:
    get:
      summary: Get Progress
      description: Get progress.
      operationId: getProgress
      x-api-path-slug: progressid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Progress
  /progress/download/{id}:
    get:
      summary: Get Progress Download
      description: Get progress download.
      operationId: getProgressDownload
      x-api-path-slug: progressdownloadid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Progress
      - Download
  /repos/settings/{repoOwner}/{repoName}:
    get:
      summary: Get Repos Settings Repoowner Reponame
      description: Get repos settings repoowner reponame.
      operationId: getReposSettingsRepoownerReponame
      x-api-path-slug: repossettingsrepoownerreponame-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Settings
      - Repoowner
      - Reponame
  /repos/settings:
    post:
      summary: Post Repos Settings
      description: Post repos settings.
      operationId: postReposSettings
      x-api-path-slug: repossettings-post
      parameters:
      - in: body
        name: settings
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Settings
  /images:
    get:
      summary: Get Images
      description: Get images.
      operationId: getImages
      x-api-path-slug: images-get
      responses:
        200:
          description: OK
      tags:
      - Images
  /images/external:
    post:
      summary: Post Images External
      description: Post images external.
      operationId: postImagesExternal
      x-api-path-slug: imagesexternal-post
      responses:
        200:
          description: OK
      tags:
      - Images
      - External
    parameters:
      summary: Parameters Images External
      description: Parameters images external.
      operationId: parametersImagesExternal
      x-api-path-slug: imagesexternal-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Images
      - External
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