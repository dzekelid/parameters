---
swagger: "2.0"
info:
  title: Heroku Parameters Application PS Restart
  description: Parameters application ps restart.
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
  /apps/{app}/ps/restart:
    parameters:
      summary: Parameters Application PS Restart
      description: Parameters application ps restart
      operationId: parametersAppsAppPsRestart
      responses:
        200:
          description: OK
      tags:
      - parameters
      - application
      - ps
      - restart
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