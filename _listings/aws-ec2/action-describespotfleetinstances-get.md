---
swagger: "2.0"
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeSpotFleetInstances&k=1:
    get:
      summary: Describe Spot Fleet Instances
      description: Describes the running instances for the specified Spot fleet
      operationId: describespotfleetinstances
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
        type: string
      - in: query
        name: EventType
        description: The type of events to describe
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return in a single call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of results
        type: string
      - in: query
        name: SpotFleetRequestId
        description: The ID of the Spot fleet request
        type: string
      - in: query
        name: StartTime
        description: The starting date and time for the events, in UTC format (for
          example, YYYY-MM-DDTHH:MM:SSZ)
        type: string
      responses:
        200:
          description: OK
      tags:
      - spot fleet instance
definitions: []
x-collection-name: AWS EC2
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