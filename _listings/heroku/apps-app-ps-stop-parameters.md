---
swagger: "2.0"
info:
  title: Heroku Parameters Application PS Stop
  description: Parameters application ps stop.
  version: "1"
host: api.heroku.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apps/{app}/ps/stop:
    parameters:
      summary: Parameters Application PS Stop
      description: Parameters application ps stop
      operationId: parametersAppsAppPsStop
      responses:
        200:
          description: OK
      tags:
      - parameters
      - application
      - ps
      - stop
definitions: []
x-collection-name: Heroku
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