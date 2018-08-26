---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /displaygroup/{displayGroupId}/media/unassign:
    post:
      summary: Unassign one or more Media items from a Display Group
      description: Removes the provided from the Display Group
      operationId: displayGroupMediaUnassign
      x-api-path-slug: displaygroupdisplaygroupidmediaunassign-post
      parameters:
      - in: path
        name: displayGroupId
        description: The Display Group to unassign from
      - in: formData
        name: mediaId
        description: The Media Ids to unassign
      responses:
        200:
          description: OK
      tags:
      - Unassign
      - More
      - Media
      - Items
      - From
      - Display
      - Group
  /displaygroup/{displayGroupId}/layout/unassign:
    post:
      summary: Unassign one or more Layout items from a Display Group
      description: Removes the provided from the Display Group
      operationId: displayGroupLayoutUnassign
      x-api-path-slug: displaygroupdisplaygroupidlayoutunassign-post
      parameters:
      - in: path
        name: displayGroupId
        description: The Display Group to unassign from
      - in: formData
        name: layoutId
        description: The Layout Ids to unassign
      responses:
        200:
          description: OK
      tags:
      - Unassign
      - More
      - Layout
      - Items
      - From
      - Display
      - Group
  /template/{layoutId}:
    post:
      summary: Add a template from a Layout
      description: Use the provided layout as a base for a new template
      operationId: template.add.from.layout
      x-api-path-slug: templatelayoutid-post
      parameters:
      - in: formData
        name: description
        description: A description of the Template
      - in: formData
        name: includeWidgets
        description: Flag indicating whether to include the widgets in the Template
      - in: path
        name: layoutId
        description: The Layout ID
      - in: formData
        name: name
        description: The Template Name
      - in: formData
        name: tags
        description: Comma separated list of Tags for the template
      responses:
        200:
          description: OK
      tags:
      - Template
      - From
      - Layout
---