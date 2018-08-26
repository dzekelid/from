---
swagger: "2.0"
x-collection-name: HERE
x-complete: 0
info:
  title: HERE Public Transit API Next Nearby Departures from a Station
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
  version: 1.0.0
host: cit.transit.api.here.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /metarouter/rest/boardservice/v2/stationboard.json:
    get:
      summary: Next Nearby Departures from a Station
      description: "*Request a list of next departure times and destinations of a
        particular station*\n\nNext nearby departures can be requested using the `metarouter/rest/boardservice/v2/stationboard.json`
        and specifying a `time` and `stnId`.\n  \n  The station ID (stnId) can be
        obtained from making a prior call to one of the station search (by name or
        by geo-coordinates) endpoints.\n\n\n\n* **lang**  `text`\n \\- Language of
        the response\n\n* **stnId**  `number`\n \\- Station Id.  The format of a station
        Id is 123456789#100. Only the first 9-digits are mandatory and if the full
        Id is to be used, the `#` character must be encoded as `%23`.      \n\n* **time**
        \ `text`\n \\- Time in format `yyyy-mm-ddThh:mm:ss`.\n\n* **strict**  `enum`\n
        \\- When `strict=1` the board will include only departures from the given
        station id.\n\n    Valid values are : `0` - disabled, `1` - enabled\n\n* **app_id**
        \ `text`\n \\- A 20 bytes Base64 URL-safe encoded string used for the authentication
        of the client application.    You must include an app_code and app_code with
        every request.\n\n* **app_code**  `text`\n \\- A 20 bytes Base64 URL-safe
        encoded string used for the authentication of the client application.    You
        must include an app_code and app_code with every request."
      operationId: MetarouterRestBoardserviceV2StationboardJsonGet
      x-api-path-slug: metarouterrestboardservicev2stationboard-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: lang
      - in: query
        name: stnId
      - in: query
        name: strict
      - in: query
        name: time
      responses:
        200:
          description: OK
      tags:
      - Next
      - Nearby
      - Departures
      - From
      - Station
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