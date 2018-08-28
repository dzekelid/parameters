swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 1
info:
  title: AWS OpsWorks API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeStackProvisioningParameters:
    get:
      summary: Describe Stack Provisioning Parameters
      description: Requests a description of a stack's provisioning parameters.
      operationId: describeStackProvisioningParameters
      x-api-path-slug: actiondescribestackprovisioningparameters-get
      parameters:
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Stack
      - Provisioning
      - Parameters