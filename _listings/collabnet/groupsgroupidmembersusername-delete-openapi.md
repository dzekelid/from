---
swagger: "2.0"
x-collection-name: CollabNet
x-complete: 0
info:
  title: CollabNet TeamForge API Documentation Removes a user from usergroup
  version: 1.0.0
  description: Removes a user from usergroup.
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /roles/{roleid}/members/{username}:
    delete:
      summary: Removes user from a role
      description: Removes user from a role.
      operationId: removeRoleMember
      x-api-path-slug: rolesroleidmembersusername-delete
      parameters:
      - in: path
        name: roleid
        description: Role identifier
      - in: path
        name: username
        description: username
      responses:
        200:
          description: OK
      tags:
      - Removes
      - User
      - From
      - Role
  /projects/{projectid}/roles/{roleid}/members/{username}:
    delete:
      summary: Removes user from a project role
      description: Removes user from a project role.
      operationId: removeUserFromProjectRole
      x-api-path-slug: projectsprojectidrolesroleidmembersusername-delete
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      - in: path
        name: roleid
        description: Role identifier
      - in: path
        name: username
        description: username
      responses:
        200:
          description: OK
      tags:
      - Removes
      - User
      - From
      - Project
      - Role
  /projectgroups/{projectgroupid}/projects/{projectid}:
    delete:
      summary: Removes project from group
      description: Removes project from group.
      operationId: removeProjectFromGroup
      x-api-path-slug: projectgroupsprojectgroupidprojectsprojectid-delete
      parameters:
      - in: path
        name: projectgroupid
        description: Project group identifier
      - in: path
        name: projectid
        description: Project identifier
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Project
      - From
      - Group
  /groups/{groupid}/members/{username}:
    delete:
      summary: Removes a user from usergroup
      description: Removes a user from usergroup.
      operationId: removeUserGroupMember
      x-api-path-slug: groupsgroupidmembersusername-delete
      parameters:
      - in: path
        name: groupid
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Removes
      - User
      - From
      - Usergroup
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