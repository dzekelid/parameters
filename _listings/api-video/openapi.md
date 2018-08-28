swagger: "2.0"
x-collection-name: api.video
x-complete: 1
info:
  title: api.video
  description: the-simplest-way-to-put-video-on-the-web
  version: 1.0.0
host: ws.api.video
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /videos/{id}/thumbnail:
    parameters:
      summary: Parameters Videos Thumbnail
      description: Parameters videos thumbnail.
      operationId: parametersVeosThumbnail
      x-api-path-slug: videosidthumbnail-parameters
      responses:
        200:
          description: Successful response
      tags:
      - Parameters
      - Videos
      - Thumbnail
  /videos/{videoId}:
    parameters:
      summary: Parameters Videos Videoid
      description: Parameters videos videoid.
      operationId: parametersVeosVeo
      x-api-path-slug: videosvideoid-parameters
      responses:
        200:
          description: Successful response
      tags:
      - Parameters
      - Videos
  /players/{id}:
    parameters:
      summary: Parameters Players
      description: Parameters players.
      operationId: parametersPlayers
      x-api-path-slug: playersid-parameters
      responses:
        200:
          description: Successful response
      tags:
      - Parameters
      - Players
  /videos/{id}:
    parameters:
      summary: Parameters Videos
      description: Parameters videos.
      operationId: parametersVeos
      x-api-path-slug: videosid-parameters
      responses:
        200:
          description: Successful response
      tags:
      - Parameters
      - Videos
  /videos/{id}/source:
    parameters:
      summary: Parameters Videos Source
      description: Parameters videos source.
      operationId: parametersVeosSource
      x-api-path-slug: videosidsource-parameters
      responses:
        200:
          description: Successful response
      tags:
      - Parameters
      - Videos
      - Source