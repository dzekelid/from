---
swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 1
info:
  title: AWS Internet of Things API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateCertificateFromCsr:
    get:
      summary: Create Certificate From Csr
      description: Creates an X.
      operationId: createCertificateFromCsr
      x-api-path-slug: actioncreatecertificatefromcsr-get
      parameters:
      - in: query
        name: certificateSigningRequest
        description: The certificate signing request (CSR)
        type: string
      - in: query
        name: setAsActive
        description: Specifies whether the certificate is active
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
---