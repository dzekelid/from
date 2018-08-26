---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Post Projects Fork Forked From
  version: 1.0.0
  description: Mark this project as forked from another
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/fork/{forked_from_id}:
    post:
      summary: Post Projects Fork Forked From
      description: Mark this project as forked from another
      operationId: postV3ProjectsIdForkForkedFromId
      x-api-path-slug: v3projectsidforkforked-from-id-post
      parameters:
      - in: path
        name: forked_from_id
        description: The ID of the project it was forked from
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Fork
      - Forked
      - From
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