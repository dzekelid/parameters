---
swagger: "2.0"
x-collection-name: The TVDB
x-complete: 0
info:
  title: The TVDB Get Series Images Query Params
  description: Returns the allowed query keys for the `/series/{id}/images/query`
    route. Contains a parameter record for each unique `keyType`, listing values that
    will return results.
  version: 2.1.2
host: api-dev.thetvdb.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search/series/params:
    get:
      summary: Get Search Series Params
      description: Returns an array of parameters to query by in the `/search/series`
        route.
      operationId: search.series.params.get
      x-api-path-slug: searchseriesparams-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - Search
      - Series
      - Params
  /series/{id}/episodes/query/params:
    get:
      summary: Get Series Episodes Query Params
      description: Returns the allowed query keys for the `/series/{id}/episodes/query`
        route
      operationId: series.id.episodes.query.params.get
      x-api-path-slug: seriesidepisodesqueryparams-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Episodes
      - Query
      - Params
  /series/{id}/filter/params:
    get:
      summary: Get Series Filter Params
      description: Returns the list of keys available for the `/series/{id}/filter`
        route
      operationId: series.id.filter.params.get
      x-api-path-slug: seriesidfilterparams-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Filter
      - Params
  /series/{id}/images/query/params:
    get:
      summary: Get Series Images Query Params
      description: Returns the allowed query keys for the `/series/{id}/images/query`
        route. Contains a parameter record for each unique `keyType`, listing values
        that will return results.
      operationId: series.id.images.query.params.get
      x-api-path-slug: seriesidimagesqueryparams-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Television
      - Series
      - Images
      - Query
      - Params
  /updated/query/params:
    get:
      summary: Get Updated Query Params
      description: Returns an array of valid query keys for the `/updated/query/params`
        route.
      operationId: updated.query.params.get
      x-api-path-slug: updatedqueryparams-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - Updated
      - Query
      - Params
  /user/ratings/query/params:
    get:
      summary: Get User Ratings Query Params
      description: Returns a list of query params for use in the `/user/ratings/query`
        route.
      operationId: user.ratings.query.params.get
      x-api-path-slug: userratingsqueryparams-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Ratings
      - Query
      - Params
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