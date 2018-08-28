swagger: "2.0"
x-collection-name: AWS Certificate Manager
x-complete: 1
info:
  title: AWS Certificate Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RemoveTagsFromCertificate:
    get:
      summary: Remove Tags From Certificate
      description: Remove one or more tags from an ACM Certificate.
      operationId: RemoveTagsFromCertificate
      x-api-path-slug: actionremovetagsfromcertificate-get
      parameters:
      - in: query
        name: CertificateArn
        description: String that contains the ARN of the ACM Certificate with one
          or more tags that you want      to remove
        type: string
      - in: query
        name: Tags
        description: The key-value pair that defines the tag to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificate Tags