---
name: HERE
x-slug: here
description: HERE Technologies enables people, enterprises and cities around the world
  to harness the power of location and create innovative solutions that make our lives
  safer and more efficient. We transform information from devices, vehicles, infrastructure
  and...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
x-kinRank: "7"
x-alexaRank: "3011"
tags: From
created: "2018-08-25"
modified: "2018-08-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/from/master/_listings/here/apis.md
specificationVersion: "0.14"
apis:
- name: Public Transport API - Next Nearby Departures from a Station
  x-api-slug: metarouterrestboardservicev2stationboard-json-get
  description: "*Request a list of next departure times and destinations of a particular
    station*\n\nNext nearby departures can be requested using the `metarouter/rest/boardservice/v2/stationboard.json`
    and specifying a `time` and `stnId`.\n  \n  The station ID (stnId) can be obtained
    from making a prior call to one of the station search (by name or by geo-coordinates)
    endpoints.\n\n\n\n* **lang**  `text`\n \\- Language of the response\n\n* **stnId**
    \ `number`\n \\- Station Id.  The format of a station Id is 123456789#100. Only
    the first 9-digits are mandatory and if the full Id is to be used, the `#` character
    must be encoded as `%23`.      \n\n* **time**  `text`\n \\- Time in format `yyyy-mm-ddThh:mm:ss`.\n\n*
    **strict**  `enum`\n \\- When `strict=1` the board will include only departures
    from the given station id.\n\n    Valid values are : `0` - disabled, `1` - enabled\n\n*
    **app_id**  `text`\n \\- A 20 bytes Base64 URL-safe encoded string used for the
    authentication of the client application.    You must include an app_code and
    app_code with every request.\n\n* **app_code**  `text`\n \\- A 20 bytes Base64
    URL-safe encoded string used for the authentication of the client application.
    \   You must include an app_code and app_code with every request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://cit.transit.api.here.com//
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/from/master/_listings/here/metarouterrestboardservicev2stationboard-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/from/master/_listings/here/metarouterrestboardservicev2stationboard-json-get-openapi.md
- name: Public Transport API - All Next Departures from a Location
  x-api-slug: metarouterrestboardservicev1multiboardby-geocoord-json-get
  description: "*Request a list of all next departure times and destinations from
    a given location.*\n\nAll next departures from a given location can be requested
    using the `metarouter/rest/boardservice/v1/multiboard/by_geocoord.json` and specifying
    a `time` and `coordinates. `The maximum numbers of nearby stations and number
    of departures per station can be restricted by using the `max_stn` and `max` parameters,
    respectively.\n  \n\n\n\n* **lang**  `text`\n \\- Language of the response\n\n*
    **startX**  `number`\n \\- The longitude of the center point of your search.    e.g.
    `13.377`\n\n* **startY**  `number`\n \\- The latitude of the center point of your
    search.    e.g. `52.515`\n\n* **time**  `text`\n \\- Time in format `yyyy-mm-ddThh:mm:ss`.\n\n*
    **app_id**  `text`\n \\- A 20 bytes Base64 URL-safe encoded string used for the
    authentication of the client application.    You must include an app_code and
    app_code with every request.\n\n* **app_code**  `text`\n \\- A 20 bytes Base64
    URL-safe encoded string used for the authentication of the client application.
    \   You must include an app_code and app_code with every request.\n\n* **max**
    \ `text`\n \\- The  maximum number of next departures per station to be included
    in the response.     The default value is 40.  \n\n* **max_stn**  `text`\n \\-
    \ The maximum number of stations for which departures are required.     The default
    value is 40.    \n\n* **prod**  `text`\n \\- A 16-bit binary number, where each
    bit represents one type of transit.  \n  0: High-speed Trains  \n  1: Intercity/EuroCity
    Trains  \n  2: Inter-regional and fast trains  \n  3: Regional and other trains
    \ \n  4: City trains  \n  5: Buses  \n  6: Boat/Ferries  \n  7: Metro/Subway  \n
    \ 8: Tram  \n  9: Ordered services/Taxi  \n  10: Inclined/Funicular  \n  11: Aerial/Cable
    Car  \n  12: Rapid Bus  \n  13: Monorail  \n  14: Air plane  \n  15: Not yet defined
    \ \n  The default is 1111111111111111, meaning all supported transit types are
    permitted."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://cit.transit.api.here.com//
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/from/master/_listings/here/metarouterrestboardservicev1multiboardby-geocoord-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/from/master/_listings/here/metarouterrestboardservicev1multiboardby-geocoord-json-get-openapi.md
x-common:
- type: x-blog-rss
  url: https://developer.here.com/blog/feed
- type: x-github
  url: https://github.com/heremaps
- type: x-postman-collection
  url: https://github.com/heremaps/postman-collections
- type: x-api-gallery
  url: http://healthcare.gov.api.gallery.streamdata.io
- type: x-api-stack
  url: http://here.stack.network
- type: x-blog
  url: https://developer.here.com/blog
- type: x-crunchbase
  url: https://crunchbase.com/organization/here-inc
- type: x-developer
  url: https://developer.here.com
- type: x-email
  url: dirk.popp@here.com
- type: x-email
  url: sebastian.kurme@here.com
- type: x-email
  url: jordan.stark@here.com
- type: x-email
  url: amy.stupavsky@here.com
- type: x-email
  url: minna.laub@here.com
- type: x-email
  url: stefanie.sirc@here.com
- type: x-email
  url: rachel.kuta@here.com
- type: x-email
  url: laurel.davis-lyons@here.com
- type: x-email
  url: linda.bradley@here.com
- type: x-email
  url: press@here.com
- type: x-twitter
  url: https://twitter.com/here
- type: x-website
  url: https://here.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---