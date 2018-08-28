---
swagger: "2.0"
x-collection-name: AWS ElastiCache
x-complete: 0
info:
  title: Amazon ElastiCache API Remove Tags From Resource
  version: 1.0.0
  description: "Removes the tags identified by the TagKeys \n            list from
    the named resource."
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: "Removes the tags identified by the TagKeys \n            list
        from the named resource."
      operationId: removeTagsFromResource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceName
        description: The Amazon Resource Name (ARN) of the resource from which you
          want the tags removed,             for example arn:aws:elasticache:us-west-2:0123456789:cluster:myCluster             or
          arn:aws:elasticache:us-west-2:0123456789:snapshot:mySnapshot
        type: string
      - in: query
        name: TagKeys.member.N
        description: A list of TagKeys identifying the tags you want removed from
          the named resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Tags
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