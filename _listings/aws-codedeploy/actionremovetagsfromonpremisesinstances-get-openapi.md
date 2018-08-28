---
swagger: "2.0"
x-collection-name: AWS CodeDeploy
x-complete: 0
info:
  title: AWS CodeDeploy API Remove Tags From On Premises Instances
  version: 1.0.0
  description: Removes one or more tags from one or more on-premises instances.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RemoveTagsFromOnPremisesInstances:
    get:
      summary: Remove Tags From On Premises Instances
      description: Removes one or more tags from one or more on-premises instances.
      operationId: removeTagsFromOnPremisesInstances
      x-api-path-slug: actionremovetagsfromonpremisesinstances-get
      parameters:
      - in: query
        name: instanceNames
        description: The names of the on-premises instances from which to remove tags
        type: string
      - in: query
        name: tags
        description: The tag key-value pairs to remove from the on-premises instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - On Premises Instances
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