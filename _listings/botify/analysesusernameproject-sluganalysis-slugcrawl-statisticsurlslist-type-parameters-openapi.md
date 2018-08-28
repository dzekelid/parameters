---
swagger: "2.0"
x-collection-name: Botify
x-complete: 0
info:
  title: Botify Parameters Analyses Username Project Slug Analysis Slug Crawl Statistics
    Urls List Type
  description: Parameters analyses username project slug analysis slug crawl statistics
    urls list type.
  version: 1.0.0
host: api.botify.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /analyses/{username}/{project_slug}:
    parameters:
      summary: Parameters Analyses Username Project Slug
      description: Parameters analyses username project slug.
      operationId: parametersAnalysesUsernameProjectSlug
      x-api-path-slug: analysesusernameproject-slug-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
  /analyses/{username}/{project_slug}/{analysis_slug}:
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug
      description: Parameters analyses username project slug analysis slug.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlug
      x-api-path-slug: analysesusernameproject-sluganalysis-slug-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
  /analyses/{username}/{project_slug}/{analysis_slug}/crawl_statistics:
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Crawl Statistics
      description: Parameters analyses username project slug analysis slug crawl statistics.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugCrawlStatistics
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statistics-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
  /analyses/{username}/{project_slug}/{analysis_slug}/crawl_statistics/time:
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Crawl Statistics
        Time
      description: Parameters analyses username project slug analysis slug crawl statistics
        time.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugCrawlStatisticsTime
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statisticstime-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
      - Time
  /analyses/{username}/{project_slug}/{analysis_slug}/crawl_statistics/urls/{list_type}:
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Crawl Statistics
        Urls List Type
      description: Parameters analyses username project slug analysis slug crawl statistics
        urls list type.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugCrawlStatisticsUrlsListType
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statisticsurlslist-type-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
      - Urls
      - List
      - Type
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