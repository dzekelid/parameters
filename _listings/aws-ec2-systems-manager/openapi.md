---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 1
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
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
---