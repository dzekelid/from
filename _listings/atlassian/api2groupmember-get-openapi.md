---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get users from group
  description: |-
    Returns all users in a group. Users are ordered by username.

    **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
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