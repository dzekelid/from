---
swagger: "2.0"
x-collection-name: AWS Route 53
x-complete: 1
info:
  title: AWS Route 53 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2013-04-01/hostedzone/Id/deauthorizevpcassociation:
    post:
      summary: Delete V P C Association Authorization
      description: Removes authorization to submit an AssociateVPCWithHostedZone request
        to associate a specified VPC with a hosted zone that was created by a different
        account. You must use the account that created the hosted zone to submit a
        DeleteVPCAssociationAuthorization request.ImportantSending this request only
        prevents the AWS account that created the VPC from associating the VPC with
        the Amazon Route 53 hosted zone in the future. If the VPC is already associated
        with the hosted zone, DeleteVPCAssociationAuthorization won't disassociate
        the VPC from the hosted zone. If you want to delete an existing association,
        use DisassociateVPCFromHostedZone.Send a DELETE request to the /2013-04-01/hostedzone/hosted
        zone ID/deauthorizevpcassociation resource. The request body must include
        a document with a DeleteVPCAssociationAuthorizationRequest element.
      operationId: deletevpcassociationauthorization
      x-api-path-slug: 20130401hostedzoneiddeauthorizevpcassociation-post
      parameters:
      - in: body
        name: DeleteVPCAssociationAuthorizationRequest
        description: Root level tag for the DeleteVPCAssociationAuthorizationRequest
          parameters
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: Id
        description: When removing authorization to associate a VPC that was created
          by one AWS account with a hosted zone that was created with a different
          AWS account, the ID of the hosted zone
        type: string
      - in: body
        name: VPC
        description: When removing authorization to associate a VPC that was created
          by one AWS account with a hosted zone that was created with a different
          AWS account, a complex type that includes the ID and region of the VPC
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - VPC
  /2013-04-01/hostedzone/Id/disassociatevpc:
    post:
      summary: Disassociate V P C From Hosted Zone
      description: Disassociates a VPC from a Amazon Route 53 private hosted zone.
        NoteYou can't disassociate the last VPC from a private hosted zone.Send a
        POST request to the /2013-04-01/hostedzone/hosted zone ID/disassociatevpcresource.
        The request body must include a document with a DisassociateVPCFromHostedZoneRequest
        element. The response includes a DisassociateVPCFromHostedZoneResponse element.ImportantYou
        can't disassociate a VPC from a private hosted zone when only one VPC is associated
        with the hosted zone. You also can't convert a private hosted zone into a
        public hosted zone.
      operationId: disassociatevpcfromhostedzone
      x-api-path-slug: 20130401hostedzoneiddisassociatevpc-post
      parameters:
      - in: body
        name: Comment
        description: 'Optional: A comment about the disassociation request'
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: DisassociateVPCFromHostedZoneRequest
        description: Root level tag for the DisassociateVPCFromHostedZoneRequest parameters
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: Id
        description: The ID of the private hosted zone that you want to disassociate
          a VPC from
        type: string
      - in: body
        name: VPC
        description: A complex type that contains information about the VPC that youre
          disassociatingfrom the specified hosted zone
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - VPC
---