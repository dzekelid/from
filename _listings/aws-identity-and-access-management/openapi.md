swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 1
info:
  title: AWS Identity and Access Management API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RemoveClientIDFromOpenIDConnectProvider:
    get:
      summary: Remove Client I D From Open I D Connect Provider
      description: |-
        Removes the specified client ID (also known as audience) from the list of client IDs
              registered for the specified IAM OpenID Connect (OIDC) provider resource object.
      operationId: removeClientIDFromOpenIDConnectProvider
      x-api-path-slug: actionremoveclientidfromopenidconnectprovider-get
      parameters:
      - in: query
        name: ClientID
        description: The client ID (also known as audience) to remove from the IAM
          OIDC provider resource
        type: string
      - in: query
        name: OpenIDConnectProviderArn
        description: The Amazon Resource Name (ARN) of the IAM OIDC provider resource
          to remove the client      ID from
        type: string
      responses:
        200:
          description: OK
      tags:
      - OpenID Connect Providers
  /?Action=RemoveRoleFromInstanceProfile:
    get:
      summary: Remove Role From Instance Profile
      description: Removes the specified IAM role from the specified EC2 instance
        profile.
      operationId: removeRoleFromInstanceProfile
      x-api-path-slug: actionremoverolefrominstanceprofile-get
      parameters:
      - in: query
        name: InstanceProfileName
        description: The name of the instance profile to update
        type: string
      - in: query
        name: RoleName
        description: The name of the role to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - Role From Instance Profiles
  /?Action=RemoveUserFromGroup:
    get:
      summary: Remove User From Group
      description: Removes the specified user from the specified group.
      operationId: removeUserFromGroup
      x-api-path-slug: actionremoveuserfromgroup-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group to update
        type: string
      - in: query
        name: UserName
        description: The name of the user to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - User From Groups