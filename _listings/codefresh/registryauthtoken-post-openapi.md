---
swagger: "2.0"
x-collection-name: Codefresh
x-complete: 0
info:
  title: Codefresh Post Registry Auth Token
  description: Post registry auth token.
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
  /images/{imageId}:
    get:
      summary: Get Images Imageid
      description: Get images imageid.
      operationId: getImagesImage
      x-api-path-slug: imagesimageid-get
      parameters:
      - in: path
        name: imageId
        description: id of the Image
      responses:
        200:
          description: OK
      tags:
      - Images
      - Imageid
  /images/{imageName}/tags:
    get:
      summary: Get Images Imagename Tags
      description: Get images imagename tags.
      operationId: getImagesImagenameTags
      x-api-path-slug: imagesimagenametags-get
      parameters:
      - in: path
        name: imageName
        description: name of the image
      responses:
        200:
          description: OK
      tags:
      - Images
      - Imagename
      - Tags
  /images/{internalImageId}/metadata:
    get:
      summary: Get Images Internalimageid Metadata
      description: Get images internalimageid metadata.
      operationId: getImagesInternalimageMetadata
      x-api-path-slug: imagesinternalimageidmetadata-get
      parameters:
      - in: path
        name: internalImageId
        description: id of the Image (from docker inspect)
      responses:
        200:
          description: OK
      tags:
      - Images
      - Internalimageid
      - Metadata
    post:
      summary: Post Images Internalimageid Metadata
      description: Post images internalimageid metadata.
      operationId: postImagesInternalimageMetadata
      x-api-path-slug: imagesinternalimageidmetadata-post
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: internalImageId
        description: id of the Image (from docker inspect)
      responses:
        200:
          description: OK
      tags:
      - Images
      - Internalimageid
      - Metadata
  /images/{internalImageId}/metadata/{keyName}:
    delete:
      summary: Delete Images Internalimageid Metadata Keyname
      description: Delete images internalimageid metadata keyname.
      operationId: deleteImagesInternalimageMetadataKeyname
      x-api-path-slug: imagesinternalimageidmetadatakeyname-delete
      parameters:
      - in: path
        name: internalImageId
        description: id of the Image from docker inspect
      - in: path
        name: keyName
        description: name of the metadata key
      responses:
        200:
          description: OK
      tags:
      - Images
      - Internalimageid
      - Metadata
      - Keyname
  /runtime/testit:
    post:
      summary: Post Runtime Testit
      description: Post runtime testit.
      operationId: postRuntimeTestit
      x-api-path-slug: runtimetestit-post
      parameters:
      - in: body
        name: options
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Runtime
      - Testit
  /pipelines:
    get:
      summary: Get Pipelines
      description: Get pipelines.
      operationId: getPipelines
      x-api-path-slug: pipelines-get
      responses:
        200:
          description: OK
      tags:
      - Pipelines
    post:
      summary: Post Pipelines
      description: Post pipelines.
      operationId: postPipelines
      x-api-path-slug: pipelines-post
      responses:
        200:
          description: OK
      tags:
      - Pipelines
  /pipelines/{name}:
    get:
      summary: Get Pipelines Name
      description: Get pipelines name.
      operationId: getPipelinesName
      x-api-path-slug: pipelinesname-get
      parameters:
      - in: path
        name: name
        description: Name of pipeline
      responses:
        200:
          description: OK
      tags:
      - Pipelines
      - Name
    put:
      summary: Put Pipelines Name
      description: Put pipelines name.
      operationId: putPipelinesName
      x-api-path-slug: pipelinesname-put
      parameters:
      - in: path
        name: name
        description: Name of pipeline
      responses:
        200:
          description: OK
      tags:
      - Pipelines
      - Name
    delete:
      summary: Delete Pipelines Name
      description: Delete pipelines name.
      operationId: deletePipelinesName
      x-api-path-slug: pipelinesname-delete
      parameters:
      - in: path
        name: name
        description: Name of pipeline
      responses:
        200:
          description: OK
      tags:
      - Pipelines
      - Name
  /admin/accounts:
    get:
      summary: Get Admin Accounts
      description: Get admin accounts.
      operationId: getAdminAccounts
      x-api-path-slug: adminaccounts-get
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Accounts
    post:
      summary: Post Admin Accounts
      description: Post admin accounts.
      operationId: postAdminAccounts
      x-api-path-slug: adminaccounts-post
      parameters:
      - in: body
        name: account
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Accounts
  /admin/accounts/{id}:
    get:
      summary: Get Admin Accounts
      description: Get admin accounts.
      operationId: getAdminAccounts
      x-api-path-slug: adminaccountsid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Accounts
    delete:
      summary: Delete Admin Accounts
      description: Delete admin accounts.
      operationId: deleteAdminAccounts
      x-api-path-slug: adminaccountsid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Accounts
  /admin/accounts/{id}/update:
    post:
      summary: Post Admin Accounts Update
      description: Post admin accounts update.
      operationId: postAdminAccountsUpdate
      x-api-path-slug: adminaccountsidupdate-post
      parameters:
      - in: body
        name: accountDetails
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Accounts
  /admin/accounts/addpendinguser:
    post:
      summary: Post Admin Accounts Addpendinguser
      description: Post admin accounts addpendinguser.
      operationId: postAdminAccountsAddpendinguser
      x-api-path-slug: adminaccountsaddpendinguser-post
      parameters:
      - in: body
        name: newUser
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Accounts
      - Pendinguser
  /accounts/{id}/users:
    get:
      summary: Get Accounts Users
      description: Get accounts users.
      operationId: getAccountsUsers
      x-api-path-slug: accountsidusers-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Users
  /accounts/{id}/update:
    post:
      summary: Post Accounts Update
      description: Post accounts update.
      operationId: postAccountsUpdate
      x-api-path-slug: accountsidupdate-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: updateData
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /accounts/{id}/adduser:
    post:
      summary: Post Accounts Adduser
      description: Post accounts adduser.
      operationId: postAccountsAdduser
      x-api-path-slug: accountsidadduser-post
      parameters:
      - in: body
        name: newUser
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - User
  /accounts/{accountId}/{userId}/adduser:
    post:
      summary: Post Accounts Adduser
      description: Post accounts adduser.
      operationId: postAccountsAccountUserAdduser
      x-api-path-slug: accountsaccountiduseridadduser-post
      parameters:
      - in: path
        name: accountId
        description: id of an object
      - in: path
        name: userId
        description: id of an object
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - User
  /accounts/{accountId}/{userId}:
    delete:
      summary: Delete Accounts
      description: Delete accounts.
      operationId: deleteAccountsAccountUser
      x-api-path-slug: accountsaccountiduserid-delete
      parameters:
      - in: path
        name: accountId
        description: id of an object
      - in: path
        name: userId
        description: id of an object
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /accounts/{id}/updateuser:
    post:
      summary: Post Accounts Updateuser
      description: Post accounts updateuser.
      operationId: postAccountsUpdateuser
      x-api-path-slug: accountsidupdateuser-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: userDetails
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - User
  /accounts/{accountId}/{userId}/admin:
    post:
      summary: Post Accounts Admin
      description: Post accounts admin.
      operationId: postAccountsAccountUserAdmin
      x-api-path-slug: accountsaccountiduseridadmin-post
      parameters:
      - in: path
        name: accountId
        description: id of an object
      - in: path
        name: userId
        description: id of an object
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Admin
    delete:
      summary: Delete Accounts Admin
      description: Delete accounts admin.
      operationId: deleteAccountsAccountUserAdmin
      x-api-path-slug: accountsaccountiduseridadmin-delete
      parameters:
      - in: path
        name: accountId
        description: id of an object
      - in: path
        name: userId
        description: id of an object
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Admin
  /providers/github/hook:
    post:
      summary: Post Provers Github Hook
      description: Post provers github hook.
      operationId: postProversGithubHook
      x-api-path-slug: providersgithubhook-post
      parameters:
      - in: body
        name: after
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: commits
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: head_commit
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: ref
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: repository
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: send-mail-and-update-github
        description: will this hook send notification to related users
      - in: body
        name: sender
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: x-github-delivery
        description: the id from github
      - in: header
        name: x-github-event
        description: event type of this hook
      - in: header
        name: x-github-signature
        description: the signature from github
      responses:
        200:
          description: OK
      tags:
      - Provers
      - Github
      - Hook
  /builds/{buildId}:
    get:
      summary: Get Builds Buildid
      description: Get builds buildid.
      operationId: getBuildsBuild
      x-api-path-slug: buildsbuildid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Builds
      - Buildid
  /builds/{serviceId}:
    post:
      summary: Post Builds Serviceid
      description: Post builds serviceid.
      operationId: postBuildsService
      x-api-path-slug: buildsserviceid-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: options
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Builds
      - Serviceid
  /builds/{buildId}/update:
    post:
      summary: Post Builds Buildid Update
      description: Post builds buildid update.
      operationId: postBuildsBuildUpdate
      x-api-path-slug: buildsbuildidupdate-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: options
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Builds
      - Buildid
  /builds:
    get:
      summary: Get Builds
      description: Get builds.
      operationId: getBuilds
      x-api-path-slug: builds-get
      parameters:
      - in: query
        name: account
        description: account name
      - in: query
        name: repoName
        description: repo name
      - in: query
        name: repoOwner
        description: repo owner
      responses:
        200:
          description: OK
      tags:
      - Builds
  /environments:
    get:
      summary: Get Environments
      description: Get environments.
      operationId: getEnvironments
      x-api-path-slug: environments-get
      responses:
        200:
          description: OK
      tags:
      - Environments
  /environments/{id}/status:
    get:
      summary: Get Environments Status
      description: Get environments status.
      operationId: getEnvironmentsStatus
      x-api-path-slug: environmentsidstatus-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environments
      - Status
  /environments/{id}/stop:
    get:
      summary: Get Environments Stop
      description: Get environments stop.
      operationId: getEnvironmentsStop
      x-api-path-slug: environmentsidstop-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environments
      - Stop
  /environments/{id}/start:
    get:
      summary: Get Environments Start
      description: Get environments start.
      operationId: getEnvironmentsStart
      x-api-path-slug: environmentsidstart-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environments
      - Start
  /environments/{id}/pause:
    get:
      summary: Get Environments Pause
      description: Get environments pause.
      operationId: getEnvironmentsPause
      x-api-path-slug: environmentsidpause-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environments
      - Pause
  /environments/{id}/unpause:
    get:
      summary: Get Environments Unpause
      description: Get environments unpause.
      operationId: getEnvironmentsUnpause
      x-api-path-slug: environmentsidunpause-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environments
      - Unpause
  /environments/{id}/terminate:
    get:
      summary: Get Environments Terminate
      description: Get environments terminate.
      operationId: getEnvironmentsTerminate
      x-api-path-slug: environmentsidterminate-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environments
      - Terminate
  /environments/all/terminate:
    get:
      summary: Get Environments All Terminate
      description: Get environments all terminate.
      operationId: getEnvironmentsAllTerminate
      x-api-path-slug: environmentsallterminate-get
      responses:
        200:
          description: OK
      tags:
      - Environments
      - ""
      - Terminate
  /environments/{id}/rename/{newName}:
    get:
      summary: Get Environments Rename Newname
      description: Get environments rename newname.
      operationId: getEnvironmentsRenameNewname
      x-api-path-slug: environmentsidrenamenewname-get
      parameters:
      - in: path
        name: id
        description: The ID of the environment to rename
      - in: path
        name: newName
        description: The new name to assign to the environment
      responses:
        200:
          description: OK
      tags:
      - Environments
      - Rename
      - Newname
  /payments/plans:
    get:
      summary: Get Payments Plans
      description: Get payments plans.
      operationId: getPaymentsPlans
      x-api-path-slug: paymentsplans-get
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Plans
  /payments:
    get:
      summary: Get Payments
      description: Get payments.
      operationId: getPayments
      x-api-path-slug: payments-get
      responses:
        200:
          description: OK
      tags:
      - Payments
    post:
      summary: Post Payments
      description: Post payments.
      operationId: postPayments
      x-api-path-slug: payments-post
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payments
  /compositions:
    get:
      summary: Get Compositions
      description: Get compositions.
      operationId: getCompositions
      x-api-path-slug: compositions-get
      responses:
        200:
          description: OK
      tags:
      - Compositions
    post:
      summary: Post Compositions
      description: Post compositions.
      operationId: postCompositions
      x-api-path-slug: compositions-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Compositions
  /compositions/{identifier}:
    get:
      summary: Get Compositions Entifier
      description: Get compositions entifier.
      operationId: getCompositionsEntifier
      x-api-path-slug: compositionsidentifier-get
      parameters:
      - in: path
        name: identifier
        description: id or name of a composition
      responses:
        200:
          description: OK
      tags:
      - Compositions
      - Entifier
  /compositions/{id}/duplicate:
    post:
      summary: Post Compositions Duplicate
      description: Post compositions duplicate.
      operationId: postCompositionsDuplicate
      x-api-path-slug: compositionsidduplicate-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Compositions
      - Duplicate
  /compositions/{id}:
    put:
      summary: Put Compositions
      description: Put compositions.
      operationId: putCompositions
      x-api-path-slug: compositionsid-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: payload
        description: Update the name/variables/body of the composition with the id
          inserted
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Compositions
    delete:
      summary: Delete Compositions
      description: Delete compositions.
      operationId: deleteCompositions
      x-api-path-slug: compositionsid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Compositions
  /compositions/{identifier}/run:
    post:
      summary: Post Compositions Entifier Run
      description: Post compositions entifier run.
      operationId: postCompositionsEntifierRun
      x-api-path-slug: compositionsidentifierrun-post
      parameters:
      - in: path
        name: identifier
        description: id or name of a composition
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Compositions
      - Entifier
      - Run
  /workflow/{repoOwner}/{repoName}/file:
    post:
      summary: Post Workflow Repoowner Reponame File
      description: Post workflow repoowner reponame file.
      operationId: postWorkflowRepoownerReponameFile
      x-api-path-slug: workflowrepoownerreponamefile-post
      parameters:
      - in: body
        name: options
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: repoName
        description: The name of the repo
      - in: path
        name: repoOwner
        description: The name of the repo owner
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Repoowner
      - Reponame
      - File
  /workflow:
    get:
      summary: Get Workflow
      description: Get workflow.
      operationId: getWorkflow
      x-api-path-slug: workflow-get
      parameters:
      - in: query
        name: query
        description: Fields to search by
      responses:
        200:
          description: OK
      tags:
      - Workflow
  /features/{accountId}:
    get:
      summary: Get Features Accountid
      description: Get features accountid.
      operationId: getFeaturesAccount
      x-api-path-slug: featuresaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The ID of the account to query for feature availability
      responses:
        200:
          description: OK
      tags:
      - Features
      - Accountid
  /registry/auth/token:
    post:
      summary: Post Registry Auth Token
      description: Post registry auth token.
      operationId: postRegistryAuthToken
      x-api-path-slug: registryauthtoken-post
      parameters:
      - in: body
        name: options
        description: Description of the token
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Registry
      - Auth
      - Token
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