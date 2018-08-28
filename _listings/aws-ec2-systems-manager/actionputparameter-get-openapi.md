---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API Put Parameter
  version: 1.0.0
  description: Add one or more paramaters to the system.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeParameters:
    get:
      summary: Describe Parameters
      description: Get information about a parameter.
      operationId: describeParameters
      x-api-path-slug: actiondescribeparameters-get
      parameters:
      - in: query
        name: Filters
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameters
  /?Action=GetParameters:
    get:
      summary: Get Parameters
      description: Get a list of parameters used by the AWS account.
      operationId: getParameters
      x-api-path-slug: actiongetparameters-get
      parameters:
      - in: query
        name: Names
        description: Names of the parameters for which you want to query information
        type: string
      - in: query
        name: WithDecryption
        description: Return decrypted secure string value
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameters
  /?Action=DeleteParameter:
    get:
      summary: Delete Parameter
      description: Delete a parameter from the system.
      operationId: deleteParameter
      x-api-path-slug: actiondeleteparameter-get
      parameters:
      - in: query
        name: Name
        description: The name of the parameter to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter
  /?Action=GetParameterHistory:
    get:
      summary: Get Parameter History
      description: Query a list of all parameters used by the AWS account.
      operationId: getParameterHistory
      x-api-path-slug: actiongetparameterhistory-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: Name
        description: The name of a parameter you want to query
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: WithDecryption
        description: Return decrypted values for secure string parameters
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter
      - History
  /?Action=PutParameter:
    get:
      summary: Put Parameter
      description: Add one or more paramaters to the system.
      operationId: putParameter
      x-api-path-slug: actionputparameter-get
      parameters:
      - in: query
        name: Description
        description: Information about the parameter that you want to add to the system
        type: string
      - in: query
        name: KeyId
        description: The parameter key ID that you want to add to the system
        type: string
      - in: query
        name: Name
        description: The name of the parameter that you want to add to the system
        type: string
      - in: query
        name: Overwrite
        description: Overwrite an existing parameter
        type: string
      - in: query
        name: Type
        description: The type of parameter that you want to add to the system
        type: string
      - in: query
        name: Value
        description: The parameter value that you want to add to the system
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter
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