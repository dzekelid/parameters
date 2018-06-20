---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 1
info:
  title: AWS Redshift API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeClusterParameters:
    get:
      summary: Describe Cluster Parameters
      description: |-
        Returns a detailed list of parameters contained within the specified Amazon Redshift
                    parameter group.
      operationId: describeClusterParameters
      x-api-path-slug: actiondescribeclusterparameters-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: ParameterGroupName
        description: The name of a cluster parameter group for which to return details
        type: string
      - in: query
        name: Source
        description: The parameter types to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameters
  /?Action=DescribeDefaultClusterParameters:
    get:
      summary: Describe Default Cluster Parameters
      description: |-
        Returns a list of parameter settings for the specified parameter group
                    family.
      operationId: describeDefaultClusterParameters
      x-api-path-slug: actiondescribedefaultclusterparameters-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: ParameterGroupFamily
        description: The name of the cluster parameter group family
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameters
---