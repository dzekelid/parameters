---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Nurego Parameters Subscriptions Entitlements
  description: Parameters subscriptions entitlements.
  contact:
    name: support@nurego.com
  version: 1.0.0
host: api.nurego.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/accounts/{account_id}:
    parameters:
      summary: Parameters Accounts
      description: Parameters accounts.
      operationId: parametersV1AccountsAccount
      x-api-path-slug: v1accountsaccount-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Accounts
  /v1/organizations/{organization_id}:
    parameters:
      summary: Parameters Organizations
      description: Parameters organizations.
      operationId: parametersV1OrganizationsOrganization
      x-api-path-slug: v1organizationsorganization-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Organizations
  /v1/subscriptions/{subscription_id}:
    parameters:
      summary: Parameters Subscriptions
      description: Parameters subscriptions.
      operationId: parametersV1SubscriptionsSubscription
      x-api-path-slug: v1subscriptionssubscription-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Subscriptions
  /v1/organizations/{organization_id}/subscriptions:
    parameters:
      summary: Parameters Organizations Subscriptions
      description: Parameters organizations subscriptions.
      operationId: parametersV1OrganizationsOrganizationSubscriptions
      x-api-path-slug: v1organizationsorganization-idsubscriptions-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Organizations
      - Subscriptions
  /v1/organizations/{organization_id}/subscriptions/{subscription_id}:
    parameters:
      summary: Parameters Organizations Subscriptions
      description: Parameters organizations subscriptions.
      operationId: parametersV1OrganizationsOrganizationSubscriptionsSubscription
      x-api-path-slug: v1organizationsorganization-idsubscriptionssubscription-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Organizations
      - Subscriptions
  /v1/subscriptions/{subscription_id}/entitlements:
    parameters:
      summary: Parameters Subscriptions Entitlements
      description: Parameters subscriptions entitlements.
      operationId: parametersV1SubscriptionsSubscriptionEntitlements
      x-api-path-slug: v1subscriptionssubscription-identitlements-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Subscriptions
      - Entitlements
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