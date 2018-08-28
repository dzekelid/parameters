---
swagger: "2.0"
x-collection-name: CircleCI
x-complete: 0
info:
  title: CircleCI Parameters Project Username Project Build Num Cancel
  description: Parameters project username project build num cancel.
  version: 1.0.0
host: circleci.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /project/{username}/{project}:
    parameters:
      summary: Parameters Project Username Project
      description: Parameters project username project.
      operationId: parametersProjectUsernameProject
      x-api-path-slug: projectusernameproject-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Project
      - Username
      - Project
  /project/{username}/{project}/build-cache:
    parameters:
      summary: Parameters Project Username Project Build Cache
      description: Parameters project username project build cache.
      operationId: parametersProjectUsernameProjectBuildCache
      x-api-path-slug: projectusernameprojectbuildcache-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Project
      - Username
      - Project
      - Build
      - Cache
  /project/{username}/{project}/checkout-key:
    parameters:
      summary: Parameters Project Username Project Checkout Key
      description: Parameters project username project checkout key.
      operationId: parametersProjectUsernameProjectCheckoutKey
      x-api-path-slug: projectusernameprojectcheckoutkey-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Project
      - Username
      - Project
      - Checkout
      - Key
  /project/{username}/{project}/checkout-key/{fingerprint}:
    parameters:
      summary: Parameters Project Username Project Checkout Key Fingerprint
      description: Parameters project username project checkout key fingerprint.
      operationId: parametersProjectUsernameProjectCheckoutKeyFingerprint
      x-api-path-slug: projectusernameprojectcheckoutkeyfingerprint-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Project
      - Username
      - Project
      - Checkout
      - Key
      - Fingerprint
  /project/{username}/{project}/envvar:
    parameters:
      summary: Parameters Project Username Project Envvar
      description: Parameters project username project envvar.
      operationId: parametersProjectUsernameProjectEnvvar
      x-api-path-slug: projectusernameprojectenvvar-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Project
      - Username
      - Project
      - Envvar
  /project/{username}/{project}/envvar/{name}:
    parameters:
      summary: Parameters Project Username Project Envvar Name
      description: Parameters project username project envvar name.
      operationId: parametersProjectUsernameProjectEnvvarName
      x-api-path-slug: projectusernameprojectenvvarname-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Project
      - Username
      - Project
      - Envvar
      - Name
  /project/{username}/{project}/ssh-key:
    parameters:
      summary: Parameters Project Username Project Ssh Key
      description: Parameters project username project ssh key.
      operationId: parametersProjectUsernameProjectSshKey
      x-api-path-slug: projectusernameprojectsshkey-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Project
      - Username
      - Project
      - Ssh
      - Key
  /project/{username}/{project}/tree/{branch}:
    parameters:
      summary: Parameters Project Username Project Tree Branch
      description: Parameters project username project tree branch.
      operationId: parametersProjectUsernameProjectTreeBranch
      x-api-path-slug: projectusernameprojecttreebranch-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Project
      - Username
      - Project
      - Tree
      - Branch
  /project/{username}/{project}/{build_num}:
    parameters:
      summary: Parameters Project Username Project Build Num
      description: Parameters project username project build num.
      operationId: parametersProjectUsernameProjectBuildNum
      x-api-path-slug: projectusernameprojectbuild-num-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Project
      - Username
      - Project
      - Build
      - Num
  /project/{username}/{project}/{build_num}/artifacts:
    parameters:
      summary: Parameters Project Username Project Build Num Artifacts
      description: Parameters project username project build num artifacts.
      operationId: parametersProjectUsernameProjectBuildNumArtifacts
      x-api-path-slug: projectusernameprojectbuild-numartifacts-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Project
      - Username
      - Project
      - Build
      - Num
      - Artifacts
  /project/{username}/{project}/{build_num}/cancel:
    parameters:
      summary: Parameters Project Username Project Build Num Cancel
      description: Parameters project username project build num cancel.
      operationId: parametersProjectUsernameProjectBuildNumCancel
      x-api-path-slug: projectusernameprojectbuild-numcancel-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Project
      - Username
      - Project
      - Build
      - Num
      - Cancel
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