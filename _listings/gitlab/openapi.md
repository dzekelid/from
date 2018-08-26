---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
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
---