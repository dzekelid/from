---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Delete default actors from project role
  description: |-
    Removes [default actors](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-resolution-get) from the project role. You may remove either a group or user, but you cannot remove a group and a user in the same request.

    Changing a project role's default actors does not affect project role members for projects already created.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/group/member:
    get:
      summary: Get users from group
      description: |-
        Returns all users in a group. Users are ordered by username.

        **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
      operationId: com.atlassian.jira.rest.v2.issue.GroupResource.getUsersFromGroup_get
      x-api-path-slug: api2groupmember-get
      parameters:
      - in: query
        name: groupname
        description: The name of the group
      - in: query
        name: includeInactiveUsers
        description: Include inactive users
      - in: query
        name: maxResults
        description: The maximum number of users to return per page
      - in: query
        name: startAt
        description: The index of the first user to return
      responses:
        200:
          description: OK
      tags:
      - Users
      - From
      - Group
  /api/2/group/user:
    delete:
      summary: Remove user from group
      description: Removes a user from a group. **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):**
        _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
      operationId: com.atlassian.jira.rest.v2.issue.GroupResource.removeUserFromGroup_delete
      x-api-path-slug: api2groupuser-delete
      parameters:
      - in: query
        name: accountid
        description: The account id of the user to remove
      - in: header
        name: force-account-id
      - in: query
        name: groupname
        description: The name of the group
      - in: query
        name: username
        description: The username of the user to remove
      responses:
        200:
          description: OK
      tags:
      - Remove
      - User
      - From
      - Group
  /api/2/project/{projectIdOrKey}/role/{id}:
    delete:
      summary: Delete actors from project role
      description: |-
        Deletes actors from a project role for the project.

        If you want to remove default actors from the project role, see the [Delete default actors from project role](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-role-id-actors-delete) resource.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg) or _Administer Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg).
      operationId: com.atlassian.jira.rest.v2.issue.project.ProjectRoleResource.deleteActor_delete
      x-api-path-slug: api2projectprojectidorkeyroleid-delete
      parameters:
      - in: header
        name: force-account-id
      - in: query
        name: group
        description: The name of the group to remove from the project role
      - in: path
        name: id
        description: The ID of the project role
      - in: path
        name: projectIdOrKey
        description: The project ID or project key (case sensitive)
      - in: query
        name: user
        description: The user account ID of the user to remove from the project role
      responses:
        200:
          description: OK
      tags:
      - Actors
      - From
      - Project
      - Role
  /api/2/role/{id}/actors:
    delete:
      summary: Delete default actors from project role
      description: |-
        Removes [default actors](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-resolution-get) from the project role. You may remove either a group or user, but you cannot remove a group and a user in the same request.

        Changing a project role's default actors does not affect project role members for projects already created.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
      operationId: com.atlassian.jira.rest.v2.issue.project.RoleResource.deleteProjectRoleActorsFromRole_delete
      x-api-path-slug: api2roleidactors-delete
      parameters:
      - in: header
        name: force-account-id
      - in: query
        name: group
        description: The group name of the group to be removed as a default actor
      - in: path
        name: id
        description: The ID of the project role
      - in: query
        name: user
        description: The user account ID of the user to remove as a default actor
      responses:
        200:
          description: OK
      tags:
      - Default
      - Actors
      - From
      - Project
      - Role
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