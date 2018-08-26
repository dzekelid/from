---
swagger: "2.0"
x-collection-name: Transport for London Unified
x-complete: 0
info:
  title: Transport for London Unified Journey  Journey Results from to to
  description: Perform a journey planner search from the parameters specified in simple
    types.
  version: v1
host: api.tfl.gov.uk
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Journey/JourneyResults/{from}/to/{to}:
    get:
      summary: Journey  Journey Results from to to
      description: Perform a journey planner search from the parameters specified
        in simple types.
      operationId: Journey_JourneyResults
      x-api-path-slug: journeyjourneyresultsfromtoto-get
      parameters:
      - in: query
        name: accessibilityPreference
        description: The accessibility preference must be a comma separated list eg
      - in: query
        name: adjustment
        description: Time adjustment command
      - in: query
        name: alternativeCycle
        description: Option to determine whether to return alternative cycling journey
      - in: query
        name: alternativeWalking
        description: Option to determine whether to return alternative walking journey
      - in: query
        name: applyHtmlMarkup
        description: Flag to determine whether certain text (e
      - in: query
        name: bikeProficiency
        description: A comma separated list of cycling proficiency levels
      - in: query
        name: cyclePreference
        description: The cycle preference
      - in: query
        name: date
        description: The date must be in yyyyMMdd format
      - in: path
        name: from
        description: Origin of the journey
      - in: query
        name: fromName
        description: An optional name to associate with the origin of the journey
          in the results
      - in: query
        name: journeyPreference
        description: 'The journey preference eg possible options: leastinterchange
          | leasttime | leastwalking'
      - in: query
        name: maxTransferMinutes
        description: The max walking time in minutes for transfer eg
      - in: query
        name: maxWalkingMinutes
        description: The max walking time in minutes for journeys eg
      - in: query
        name: mode
        description: The mode must be a comma separated list of modes
      - in: query
        name: nationalSearch
        description: Does the journey cover stops outside London? eg
      - in: query
        name: taxiOnlyTrip
        description: A boolean to indicate whether to return one or more taxi journeys
      - in: query
        name: time
        description: The time must be in HHmm format
      - in: query
        name: timeIs
        description: 'Does the time given relate to arrival or leaving time? Possible
          options: departing | arriving'
      - in: path
        name: to
        description: Destination of the journey
      - in: query
        name: toName
        description: An optional name to associate with the destination of the journey
          in the results
      - in: query
        name: useMultiModalCall
        description: A boolean to indicate whether or not to return 3 public transport
          journeys, a bus journey, a cycle hire journey, a personal cycle journey
          and a walking journey
      - in: query
        name: via
        description: Travel through point on the journey
      - in: query
        name: viaName
        description: An optional name to associate with the via point of the journey
          in the results
      - in: query
        name: walkingOptimization
        description: A boolean to indicate whether to optimize journeys using walking
      - in: query
        name: walkingSpeed
        description: The walking speed
      responses:
        200:
          description: OK
      tags:
      - Journey
      - ""
      - Journey
      - Results
      - From
      - To
      - To
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