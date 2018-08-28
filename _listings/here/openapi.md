swagger: "2.0"
x-collection-name: HERE
x-complete: 1
info:
  title: Weather API
  description: the-here-weather-api-provides-weather-forecasts-and-reports-on-current-weather-conditions-provides-information-on-severe-weather-alerts-provides-information-about-when-the-sun-and-moon-rise-and-set-and-the-phase-of-the-moonthis-example-set-works-with-version-1-2-4-or-higheradditional-information-can-be-found-on-developer-here-comhttpsdeveloper-here-comrestapisdocumentationweather
  version: 1.0.0
host: weather.cit.api.here.com
basePath: /weather/1.0
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
  /metarouter/rest/boardservice/v1/multiboard/by_geocoord.json:
    get:
      summary: All Next Departures from a Location
      description: "*Request a list of all next departure times and destinations from
        a given location.*\n\nAll next departures from a given location can be requested
        using the `metarouter/rest/boardservice/v1/multiboard/by_geocoord.json` and
        specifying a `time` and `coordinates. `The maximum numbers of nearby stations
        and number of departures per station can be restricted by using the `max_stn`
        and `max` parameters, respectively.\n  \n\n\n\n* **lang**  `text`\n \\- Language
        of the response\n\n* **startX**  `number`\n \\- The longitude of the center
        point of your search.    e.g. `13.377`\n\n* **startY**  `number`\n \\- The
        latitude of the center point of your search.    e.g. `52.515`\n\n* **time**
        \ `text`\n \\- Time in format `yyyy-mm-ddThh:mm:ss`.\n\n* **app_id**  `text`\n
        \\- A 20 bytes Base64 URL-safe encoded string used for the authentication
        of the client application.    You must include an app_code and app_code with
        every request.\n\n* **app_code**  `text`\n \\- A 20 bytes Base64 URL-safe
        encoded string used for the authentication of the client application.    You
        must include an app_code and app_code with every request.\n\n* **max**  `text`\n
        \\- The  maximum number of next departures per station to be included in the
        response.     The default value is 40.  \n\n* **max_stn**  `text`\n \\-  The
        maximum number of stations for which departures are required.     The default
        value is 40.    \n\n* **prod**  `text`\n \\- A 16-bit binary number, where
        each bit represents one type of transit.  \n  0: High-speed Trains  \n  1:
        Intercity/EuroCity Trains  \n  2: Inter-regional and fast trains  \n  3: Regional
        and other trains  \n  4: City trains  \n  5: Buses  \n  6: Boat/Ferries  \n
        \ 7: Metro/Subway  \n  8: Tram  \n  9: Ordered services/Taxi  \n  10: Inclined/Funicular
        \ \n  11: Aerial/Cable Car  \n  12: Rapid Bus  \n  13: Monorail  \n  14: Air
        plane  \n  15: Not yet defined  \n  The default is 1111111111111111, meaning
        all supported transit types are permitted."
      operationId: MetarouterRestBoardserviceV1MultiboardByGeocoordJsonGet
      x-api-path-slug: metarouterrestboardservicev1multiboardby-geocoord-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: lang
      - in: query
        name: max
      - in: query
        name: max_stn
      - in: query
        name: prod
      - in: query
        name: startX
      - in: query
        name: startY
      - in: query
        name: time
      responses:
        200:
          description: OK
      tags:
      - All
      - Next
      - Departures
      - From
      - Location