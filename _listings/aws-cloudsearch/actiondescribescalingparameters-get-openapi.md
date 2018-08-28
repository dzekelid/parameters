---
swagger: "2.0"
x-collection-name: AWS CloudSearch
x-complete: 0
info:
  title: AWS CloudSearch Describe Scaling Parameters
  version: 1.0.0
  description: Gets the scaling parameters configured for a domain.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeScalingParameters:
    get:
      summary: Describe Scaling Parameters
      description: Gets the scaling parameters configured for a domain.
      operationId: DescribeScalingParameters
      x-api-path-slug: actiondescribescalingparameters-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scaling Parameters
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