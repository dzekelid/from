---
name: Transport for London Unified
x-slug: transport-for-london-unified
description: We are the integrated transport authority responsible for delivering
  Mayor of London Sadiq Khans strategy and commitments on transport. We run the day-to-day
  operation of the Capitals public transport network and manage Londons main roads.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/transport-for-london-unified-api.png
x-kinRank: "7"
x-alexaRank: "0"
tags: From
created: "2018-08-25"
modified: "2018-08-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/from/master/_listings/transport-for-london-unified/apis.md
specificationVersion: "0.14"
apis:
- name: Transport for London Unified - Journey  Journey Results from to to
  x-api-slug: journeyjourneyresultsfromtoto-get
  description: Perform a journey planner search from the parameters specified in simple
    types.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/transport-for-london-unified-api.png
  humanURL: https://tfl.gov.uk/
  baseURL: https://api.tfl.gov.uk//
  tags: Transportation, Transit, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/from/master/_listings/transport-for-london-unified/journeyjourneyresultsfromtoto-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/from/master/_listings/transport-for-london-unified/journeyjourneyresultsfromtoto-get-openapi.md
- name: Transport for London Unified - Line  Timetable from Stop Point Id
  x-api-slug: lineidtimetablefromstoppointid-get
  description: Gets the timetable for a specified station on the give line.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/transport-for-london-unified-api.png
  humanURL: https://tfl.gov.uk/
  baseURL: https://api.tfl.gov.uk//
  tags: Transportation, Transit, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/from/master/_listings/transport-for-london-unified/lineidtimetablefromstoppointid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/from/master/_listings/transport-for-london-unified/lineidtimetablefromstoppointid-get-openapi.md
- name: Transport for London Unified - Line  Timetable from Stop Point Id to to Stop
    Point Id
  x-api-slug: lineidtimetablefromstoppointidtotostoppointid-get
  description: Gets the timetable for a specified station on the give line with specified
    destination.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/transport-for-london-unified-api.png
  humanURL: https://tfl.gov.uk/
  baseURL: https://api.tfl.gov.uk//
  tags: Transportation, Transit, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/from/master/_listings/transport-for-london-unified/lineidtimetablefromstoppointidtotostoppointid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/from/master/_listings/transport-for-london-unified/lineidtimetablefromstoppointidtotostoppointid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://transitfeeds.api.gallery.streamdata.io
- type: x-api-stack
  url: http://transport.for.london.unified.stack.network
- type: x-developer
  url: http://api.tfl.gov.uk
- type: x-website
  url: https://tfl.gov.uk/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---