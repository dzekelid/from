---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 1
info:
  title: Global Change Information System API
  description: who-we-are-what-the-gcis-is-and-how-we-use-identifiers-and-semantic-information-to-provide-points-of-reference-and-traceability--examples-and-tutorials-for-using-this-system-as-a-researcher-citizen-scientist-application-developer-or-information-theorist--a-description-of-how-the-information-is-structured-including-the-overlaps-between-relational-and-semantic-representations-of-the-information--complete-documentation-for-the-api-including-methods-for-browsing-and-finding-resources-
  version: v1
host: data.globalchange.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lexicon/{lexicon_identifier}/find/{context}/{term}:
    get:
      summary: Lookup a GCID from a term
      description: Given a lexicon, term, and context, return a 303 redirect to a
        GCID
      operationId: given-a-lexicon-term-and-context-return-a-303-redirect-to-a-gcid
      x-api-path-slug: lexiconlexicon-identifierfindcontextterm-get
      parameters:
      - in: path
        name: context
        description: context description
      - in: path
        name: lexicon_identifier
        description: lexicon_identifier description
      - in: path
        name: term
        description: term description
      responses:
        200:
          description: OK
      tags:
      - Lookup
      - GCID
      - From
      - Term
  /lexicon/{lexicon_identifier}/{context}/{term}:
    get:
      summary: Lookup a GCID from a term
      description: Given a lexicon, term, and context, return a 303 redirect to a
        GCID
      operationId: given-a-lexicon-term-and-context-return-a-303-redirect-to-a-gcid
      x-api-path-slug: lexiconlexicon-identifiercontextterm-get
      parameters:
      - in: path
        name: context
        description: context description
      - in: path
        name: lexicon_identifier
        description: lexicon_identifier description
      - in: path
        name: term
        description: term description
      responses:
        200:
          description: OK
      tags:
      - Lookup
      - GCID
      - From
      - Term
---