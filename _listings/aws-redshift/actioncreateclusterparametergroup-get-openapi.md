---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Create Cluster Parameter Group
  version: 1.0.0
  description: Creates an Amazon Redshift parameter group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateClusterParameterGroup:
    get:
      summary: Create Cluster Parameter Group
      description: Creates an Amazon Redshift parameter group.
      operationId: createClusterParameterGroup
      x-api-path-slug: actioncreateclusterparametergroup-get
      parameters:
      - in: query
        name: Description
        description: A description of the parameter group
        type: string
      - in: query
        name: ParameterGroupFamily
        description: The Amazon Redshift engine version to which the cluster parameter
          group applies
        type: string
      - in: query
        name: ParameterGroupName
        description: The name of the cluster parameter group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
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