---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 1
info:
  title: AWS Storage Gateway Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateSnapshotFromVolumeRecoveryPoint:
    get:
      summary: Create Snapshot From Volume Recovery Point
      description: Initiates a snapshot of a gateway from a volume recovery point.
      operationId: createSnapshotFromVolumeRecoveryPoint
      x-api-path-slug: actioncreatesnapshotfromvolumerecoverypoint-get
      parameters:
      - in: query
        name: SnapshotDescription
        description: 'Type: String'
        type: string
      - in: query
        name: VolumeARN
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: Removes one or more tags from the specified resource.
      operationId: removeTagsFromResource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceARN
        description: The Amazon Resource Name (ARN) of the resource you want to remove
          the tags         from
        type: string
      - in: query
        name: TagKeys
        description: The keys of the tags you want to remove from the specified resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
---