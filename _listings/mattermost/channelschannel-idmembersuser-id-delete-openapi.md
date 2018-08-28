---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Remove user from channel
  description: |-
    Delete a channel member, effectively removing them from a channel.
    ##### Permissions
    `manage_public_channel_members` permission if the channel is public.
    `manage_private_channel_members` permission if the channel is private.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /teams/members/invite:
    post:
      summary: Add user to team from invite
      description: |-
        Using either an invite id or hash/data pair from an email invite link, add a user to a team.
        ##### Permissions
        Must be authenticated.
      operationId: using-either-an-invite-id-or-hashdata-pair-from-an-email-invite-link-add-a-user-to-a-team-permission
      x-api-path-slug: teamsmembersinvite-post
      parameters:
      - in: query
        name: data
        description: Data with time and team id
      - in: query
        name: hash
        description: Hash value with time, team id and and InviteSaltId
      - in: query
        name: invite_id
        description: Invite id to add user to the team
      responses:
        200:
          description: OK
      tags:
      - User
      - To
      - Team
      - From
      - Invite
  /teams/{team_id}/members/{user_id}:
    delete:
      summary: Remove user from team
      description: |-
        Delete the team member object for a user, effectively removing them from a team.
        ##### Permissions
        Must be logged in as the user or have the `remove_user_from_team` permission.
      operationId: delete-the-team-member-object-for-a-user-effectively-removing-them-from-a-team-permissionsmust-be-lo
      x-api-path-slug: teamsteam-idmembersuser-id-delete
      parameters:
      - in: path
        name: team_id
        description: Team GUID
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Remove
      - User
      - From
      - Team
  /teams/{team_id}/import:
    post:
      summary: Import a Team from other application
      description: |-
        Import a team into a existing team. Import users, channels, posts, hooks.
        ##### Permissions
        Must have `permission_import_team` permission.
      operationId: import-a-team-into-a-existing-team-import-users-channels-posts-hooks-permissionsmust-have-permission
      x-api-path-slug: teamsteam-idimport-post
      parameters:
      - in: formData
        name: file
        description: A file to be uploaded in zip format
      - in: formData
        name: filesize
        description: The size of the zip file to be imported
      - in: formData
        name: importFrom
        description: String that defines from which application the team was exported
          to be imported into Mattermost
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Import
      - Team
      - From
      - Other
      - Application
  /channels/{channel_id}/convert:
    post:
      summary: Convert a channel from public to private
      description: |-
        Convert into private channel from the provided channel id string.

        __Minimum server version__: 4.10

        ##### Permissions
        Must have `manage_system` permission.
      operationId: convert-into-private-channel-from-the-provided-channel-id-string-minimum-server-version--410-permiss
      x-api-path-slug: channelschannel-idconvert-post
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      responses:
        200:
          description: OK
      tags:
      - Convert
      - Channel
      - From
      - Public
      - To
      - Private
  /channels/{channel_id}/members/{user_id}:
    delete:
      summary: Remove user from channel
      description: |-
        Delete a channel member, effectively removing them from a channel.
        ##### Permissions
        `manage_public_channel_members` permission if the channel is public.
        `manage_private_channel_members` permission if the channel is private.
      operationId: delete-a-channel-member-effectively-removing-them-from-a-channel-permissionsmanage-public-channel-me
      x-api-path-slug: channelschannel-idmembersuser-id-delete
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Remove
      - User
      - From
      - Channel
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