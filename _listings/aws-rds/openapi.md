---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 1
info:
  title: AWS RDS API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeDBClusterParameters:
    get:
      summary: Describe D B Cluster Parameters
      description: Returns the detailed parameter list for a particular DB cluster
        parameter group.
      operationId: describedbclusterparameters
      x-api-path-slug: actiondescribedbclusterparameters-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of a specific DB cluster parameter group to return parameter
          details for
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      DescribeDBClusterParameters
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: Source
        description: A value that indicates to return only parameters for a specific
          source
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameters
  /?Action=DescribeDBParameters:
    get:
      summary: Describe D B Parameters
      description: Returns the detailed parameter list for a particular DB parameter
        group.
      operationId: describedbparameters
      x-api-path-slug: actiondescribedbparameters-get
      parameters:
      - in: query
        name: DBParameterGroupName
        description: The name of a specific DB parameter group to return details for
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeDBParameters
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: Source
        description: The parameter types to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameters
  /?Action=DescribeEngineDefaultClusterParameters:
    get:
      summary: Describe Engine Default Cluster Parameters
      description: Returns the default engine and system parameter information for
        the cluster database engine.
      operationId: describeenginedefaultclusterparameters
      x-api-path-slug: actiondescribeenginedefaultclusterparameters-get
      parameters:
      - in: query
        name: DBParameterGroupFamily
        description: The name of the DB cluster parameter group family to return engine
          parameter information for
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      DescribeEngineDefaultClusterParameters
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Default Cluster Parameters
  /?Action=DescribeEngineDefaultParameters:
    get:
      summary: Describe Engine Default Parameters
      description: Returns the default engine and system parameter information for
        the specified database engine.
      operationId: describeenginedefaultparameters
      x-api-path-slug: actiondescribeenginedefaultparameters-get
      parameters:
      - in: query
        name: DBParameterGroupFamily
        description: The name of the DB parameter group family
        type: string
      - in: query
        name: Filters.Filter.N
        description: Not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeEngineDefaultParameters
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Default Parameters
---