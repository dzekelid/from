---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 0
info:
  title: AWS Cognito API Unsubscribe From Dataset
  version: 1.0.0
  description: Unsubscribes from receiving notifications when a dataset is modified
    by another device.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AdminRemoveUserFromGroup:
    get:
      summary: Admin Remove User From Group
      description: Removes the specified user from the specified group.
      operationId: adminRemoveUserFromGroup
      x-api-path-slug: actionadminremoveuserfromgroup-get
      parameters:
      - in: query
        name: GroupName
        description: The group name
        type: string
      - in: query
        name: Username
        description: The username for the user
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /?Action=UnsubscribeFromDataset:
    get:
      summary: Unsubscribe From Dataset
      description: Unsubscribes from receiving notifications when a dataset is modified
        by another device.
      operationId: unsubscribeFromDataset
      x-api-path-slug: actionunsubscribefromdataset-get
      parameters:
      - in: query
        name: DatasetName
        description: The name of the dataset from which to unsubcribe
        type: string
      - in: query
        name: DeviceId
        description: The unique ID generated for this device by Cognito
        type: string
      - in: query
        name: IdentityId
        description: Unique ID for this identity
        type: string
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Dataset
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