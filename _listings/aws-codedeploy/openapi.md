swagger: "2.0"
x-collection-name: AWS CodeDeploy
x-complete: 1
info:
  title: AWS CodeDeploy API
  version: 1.0.0
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