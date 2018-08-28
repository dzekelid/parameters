swagger: "2.0"
x-collection-name: AWS CloudSearch
x-complete: 1
info:
  title: AWS CloudSearch
  version: 1.0.0
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
  /?Action=UpdateScalingParameters:
    get:
      summary: Update Scaling Parameters
      description: Configures scaling parameters for a domain.
      operationId: UpdateScalingParameters
      x-api-path-slug: actionupdatescalingparameters-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      - in: query
        name: ScalingParameters
        description: The desired instance type and desired number of replicas of each
          index partition
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scaling Parameters