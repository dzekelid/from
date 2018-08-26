---
swagger: "2.0"
x-collection-name: AWS Directory Service
x-complete: 1
info:
  title: AWS Directory Service API
  version: 1.0.0
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
      description: Removes tags from a directory.
      operationId: removeTagsFromResource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceId
        description: Identifier (ID) of the directory from which to remove the tag
        type: string
      - in: query
        name: TagKeys
        description: The tag key (name) of the tag to be removed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Tags
  /?Action=RestoreFromSnapshot:
    get:
      summary: Restore From Snapshot
      description: Restores a directory using an existing directory snapshot.
      operationId: restoreFromSnapshot
      x-api-path-slug: actionrestorefromsnapshot-get
      parameters:
      - in: query
        name: SnapshotId
        description: The identifier of the snapshot to restore from
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
---