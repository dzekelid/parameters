---
swagger: "2.0"
x-collection-name: Heroku
x-complete: 0
info:
  title: Heroku Parameters Application PS
  description: Parameters application ps.
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
  /addons:
    parameters:
      summary: Parameters Addons
      description: Parameters addons.
      operationId: parametersAddons
      x-api-path-slug: addons-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - ons
  /apps/{app}/addons/{addon}:
    parameters:
      summary: Parameters Applications Addons
      description: Parameters applications addons.
      operationId: parametersAppsAppAddonsAddon
      x-api-path-slug: appsappaddonsaddon-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Applications
      - ons
  /apps:
    parameters:
      summary: Parameters Applications
      description: Parameters applications.
      operationId: parametersApps
      x-api-path-slug: apps-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Applications
  /apps/{name}:
    parameters:
      summary: Parameters Applications Name
      description: Parameters applications name.
      operationId: parametersAppsName
      x-api-path-slug: appsname-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Applications
      - Name
  /apps/{app}/collaborators:
    parameters:
      summary: Parameters Application Collaborators
      description: Parameters application collaborators.
      operationId: parametersAppsAppCollaborators
      x-api-path-slug: appsappcollaborators-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - Collaborators
  /apps/{app}/collaborators/{email}:
    parameters:
      summary: Parameters Application Collaborators Email
      description: Parameters application collaborators email.
      operationId: parametersAppsAppCollaboratorsEmail
      x-api-path-slug: appsappcollaboratorsemail-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - Collaborators
      - Email
  /apps/{app}/config_vars:
    parameters:
      summary: Parameters Application Config Variables
      description: Parameters application config variables.
      operationId: parametersAppsAppConfigVars
      x-api-path-slug: appsappconfig-vars-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - Config
      - Variables
  /apps/{app}/config_vars/{key}:
    parameters:
      summary: Parameters Application Config Variables Key
      description: Parameters application config variables key.
      operationId: parametersAppsAppConfigVarsKey
      x-api-path-slug: appsappconfig-varskey-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - Config
      - Variables
      - Key
  /apps/{app}/domains:
    parameters:
      summary: Parameters Application Domains
      description: Parameters application domains.
      operationId: parametersAppsAppDomains
      x-api-path-slug: appsappdomains-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - Domains
  /apps/{app}/domains/{domain_name}:
    parameters:
      summary: Parameters Application Domain Name
      description: Parameters application domain name.
      operationId: parametersAppsAppDomainsDomainName
      x-api-path-slug: appsappdomainsdomain-name-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - Domain
      - Name
  /user/keys:
    parameters:
      summary: Parameters User Keys
      description: Parameters user keys.
      operationId: parametersUserKeys
      x-api-path-slug: userkeys-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - User
      - Keys
  /user/keys/{key}:
    parameters:
      summary: Parameters User Keys Key
      description: Parameters user keys key.
      operationId: parametersUserKeysKey
      x-api-path-slug: userkeyskey-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - User
      - Keys
      - Key
  /apps/{app}/logs:
    parameters:
      summary: Parameters Application Logs
      description: Parameters application logs.
      operationId: parametersAppsAppLogs
      x-api-path-slug: appsapplogs-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - Logs
  /apps/{app}/ps:
    parameters:
      summary: Parameters Application PS
      description: Parameters application ps.
      operationId: parametersAppsAppPs
      x-api-path-slug: appsappps-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - PS
  /apps/{app}/ps/restart:
    parameters:
      summary: Parameters Application PS Restart
      description: Parameters application ps restart.
      operationId: parametersAppsAppPsRestart
      x-api-path-slug: appsapppsrestart-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - PS
      - Restart
  /apps/{app}/ps/stop:
    parameters:
      summary: Parameters Application PS Stop
      description: Parameters application ps stop.
      operationId: parametersAppsAppPsStop
      x-api-path-slug: appsapppsstop-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - PS
      - Stop
  /apps/{app}/ps/scale:
    parameters:
      summary: Parameters Application PS Scale
      description: Parameters application ps scale.
      operationId: parametersAppsAppPsScale
      x-api-path-slug: appsapppsscale-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - PS
      - Scale
  /apps/{app}/releases:
    parameters:
      summary: Parameters Application Releases
      description: Parameters application releases.
      operationId: parametersAppsAppReleases
      x-api-path-slug: appsappreleases-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - Releases
  /apps/{app}/releases/{release}:
    parameters:
      summary: Parameters Application Releases
      description: Parameters application releases.
      operationId: parametersAppsAppReleasesRelease
      x-api-path-slug: appsappreleasesrelease-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - Releases
  /apps/{app}/stack:
    parameters:
      summary: Parameters Application Stack
      description: Parameters application stack.
      operationId: parametersAppsAppStack
      x-api-path-slug: appsappstack-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - Stack
  /apps/{app}/addons:
    parameters:
      summary: Parameter Application Addons
      description: Parameter application addons.
      operationId: parametersAppsAppAddons
      x-api-path-slug: appsappaddons-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameter
      - Application
      - ons
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