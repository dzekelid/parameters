---
swagger: "2.0"
x-collection-name: EPA Envirofacts
x-complete: 0
info:
  title: U.S. EPA Enforcement and Compliance History Online (ECHO) - Effluent Charting
    and Reporting ECHO CWA Parameter Lookup Service
  description: Look up Clean Water Act parameter codes and descriptions in the Integrated
    Compliance Information System - National Pollutant Discharge Elimination System
    (ICIS-NPDES) by code or term.
  contact:
    name: US EPA, OECA Integration, Targeting and Access Branch
  version: 1.0.0
host: ofmpub.epa.gov
basePath: /echo
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest_lookups.npdes_parameters:
    get:
      summary: ECHO NPDES Parameters Lookup Service
      description: ICIS Limit Parameter Code and Name lookup based on the supply of
        a partial parameter name. (NPDES = National Pollutant Discharge Elimination
        System)
      operationId: icis-limit-parameter-code-and-name-lookup-based-on-the-supply-of-a-partial-parameter-name--npdes--na
      x-api-path-slug: rest-lookups-npdes-parameters-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: output
        description: Output Format Flag
      responses:
        200:
          description: OK
      tags:
      - Environment
      - ECHO
      - NPDES
      - Parameters
      - Lookup
      - Service
  /rest_lookups.cwa_parameters:
    get:
      summary: ECHO CWA Parameter Lookup Service
      description: Look up Clean Water Act parameter codes and descriptions in the
        Integrated Compliance Information System - National Pollutant Discharge Elimination
        System (ICIS-NPDES) by code or term.
      operationId: look-up-clean-water-act-parameter-codes-and-descriptions-in-the-integrated-compliance-information-sy
      x-api-path-slug: rest-lookups-cwa-parameters-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Environment
      - ECHO
      - CWA
      - Parameter
      - Lookup
      - Service
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