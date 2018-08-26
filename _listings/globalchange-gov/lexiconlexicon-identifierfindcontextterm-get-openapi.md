---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 0
info:
  title: Global Change Information System API Lookup a GCID from a term
  description: Given a lexicon, term, and context, return a 303 redirect to a GCID
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