swagger: "2.0"
x-collection-name: TVmaze
x-complete: 1
info:
  title: TVmaze user
  description: access-to-the-user-api-is-only-possible-for-users-with-a-premiumhttpwww-tvmaze-compremium-account--a-user-can-only-access-their-own-user-data-authentication-uses-http-basic--use-the-tvmaze-username-as-authentication-username-and-the-tvmaze-api-key-as-authentication-password--your-api-key-can-be-found-on-your-dashboardhttpwww-tvmaze-comdashboard--to-try-out-these-api-calls-from-this-page-click-the-authorize-button-on-top-and-input-your-credentials-
  version: "1.0"
host: api.tvmaze.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/episodes/{episode_id}:
    parameters:
      summary: Parameters User Episodes
      description: Parameters user episodes.
      operationId: parametersUserEpisodesEpisode
      x-api-path-slug: userepisodesepisode-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Episodes
  /user/follows/networks/{network_id}:
    parameters:
      summary: Parameters User Follows Networks
      description: Parameters user follows networks.
      operationId: parametersUserFollowsNetworksNetwork
      x-api-path-slug: userfollowsnetworksnetwork-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Follows
      - Networks
  /user/follows/people/{person_id}:
    parameters:
      summary: Parameters User Follows People Person
      description: Parameters user follows people person.
      operationId: parametersUserFollowsPeoplePerson
      x-api-path-slug: userfollowspeopleperson-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Follows
      - People
      - Person
  /user/follows/shows/{show_id}:
    parameters:
      summary: Parameters User Follows Shows
      description: Parameters user follows shows.
      operationId: parametersUserFollowsShowsShow
      x-api-path-slug: userfollowsshowsshow-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Follows
      - Shows
  /user/follows/webchannels/{webchannel_id}:
    parameters:
      summary: Parameters User Follows Webchannels Webchannel
      description: Parameters user follows webchannels webchannel.
      operationId: parametersUserFollowsWebchannelsWebchannel
      x-api-path-slug: userfollowswebchannelswebchannel-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Follows
      - Webchannels
      - Webchannel
  /user/votes/episodes/{episode_id}:
    parameters:
      summary: Parameters User Votes Episodes
      description: Parameters user votes episodes.
      operationId: parametersUserVotesEpisodesEpisode
      x-api-path-slug: uservotesepisodesepisode-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Votes
      - Episodes
  /user/votes/shows/{show_id}:
    parameters:
      summary: Parameters User Votes Shows
      description: Parameters user votes shows.
      operationId: parametersUserVotesShowsShow
      x-api-path-slug: uservotesshowsshow-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Votes
      - Shows