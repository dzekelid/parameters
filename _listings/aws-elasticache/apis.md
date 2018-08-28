---
name: AWS ElastiCache
x-slug: aws-elasticache
description: Amazon ElastiCache is a web service that makes it easy to deploy, operate,
  and scale an in-memory data store or cache in the cloud. The service improves the
  performance of web applications by allowing you to retrieve information from fast,
  managed, in-memory data stores, instead of relying entirely on slower disk-based
  databases. Amazon ElastiCache automatically detects and replaces failed nodes, reducing
  the overhead associated with self-managed infrastructures and provides a resilient
  system that mitigates the risk of overloaded databases, which slow website and application
  load times. Through integration with Amazon CloudWatch, Amazon ElastiCache provides
  enhanced visibility into key performance metrics associated with your Redis or Memcached
  nodes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Parameters
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/parameters/master/_listings/aws-elasticache/apis.md
specificationVersion: "0.14"
apis:
- name: AWS ElastiCache API - Create Cache Parameter Group
  x-api-slug: actioncreatecacheparametergroup-get
  description: Creates a new cache parameter group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: :///
  tags: Amazon Web Services, Cache, Stack Network, Performance, Availability, API
    Service Provider, API Service Provider, API Provider, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/parameters/master/_listings/aws-elasticache/actioncreatecacheparametergroup-get-openapi.md
- name: AWS ElastiCache API - Delete Cache Parameter Group
  x-api-slug: actiondeletecacheparametergroup-get
  description: |-
    Deletes the specified cache parameter
                group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: :///
  tags: Amazon Web Services, Cache, Stack Network, Performance, Availability, API
    Service Provider, API Service Provider, API Provider, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/parameters/master/_listings/aws-elasticache/actiondeletecacheparametergroup-get-openapi.md
- name: AWS ElastiCache API - Describe Cache Parameter Groups
  x-api-slug: actiondescribecacheparametergroups-get
  description: |-
    Returns a list of cache parameter group
                descriptions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: :///
  tags: Amazon Web Services, Cache, Stack Network, Performance, Availability, API
    Service Provider, API Service Provider, API Provider, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/parameters/master/_listings/aws-elasticache/actiondescribecacheparametergroups-get-openapi.md
- name: AWS ElastiCache API - Describe Cache Parameters
  x-api-slug: actiondescribecacheparameters-get
  description: |-
    Returns the detailed parameter list for a
                particular cache parameter group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: :///
  tags: Amazon Web Services, Cache, Stack Network, Performance, Availability, API
    Service Provider, API Service Provider, API Provider, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/parameters/master/_listings/aws-elasticache/actiondescribecacheparameters-get-openapi.md
- name: AWS ElastiCache API - Describe Engine Default Parameters
  x-api-slug: actiondescribeenginedefaultparameters-get
  description: |-
    Returns the default engine and
                system parameter information for the specified cache engine.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: :///
  tags: Amazon Web Services, Cache, Stack Network, Performance, Availability, API
    Service Provider, API Service Provider, API Provider, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/parameters/master/_listings/aws-elasticache/actiondescribeenginedefaultparameters-get-openapi.md
- name: AWS ElastiCache API - Modify Cache Parameter Group
  x-api-slug: actionmodifycacheparametergroup-get
  description: |-
    Modifies the parameters of a cache
                parameter group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: :///
  tags: Amazon Web Services, Cache, Stack Network, Performance, Availability, API
    Service Provider, API Service Provider, API Provider, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/parameters/master/_listings/aws-elasticache/actionmodifycacheparametergroup-get-openapi.md
- name: AWS ElastiCache API - Reset Cache Parameter Group
  x-api-slug: actionresetcacheparametergroup-get
  description: |-
    Modifies the parameters of a cache
                parameter group to the engine or system default value.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: :///
  tags: Amazon Web Services, Cache, Stack Network, Performance, Availability, API
    Service Provider, API Service Provider, API Provider, Profiles, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/parameters/master/_listings/aws-elasticache/actionresetcacheparametergroup-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.elastic.mapreduce.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.elasticache.stack.network
- type: x-documentation
  url: http://docs.aws.amazon.com/AmazonElastiCache/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/elasticache/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/elasticache/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/elasticache/pricing/
- type: x-resources
  url: https://aws.amazon.com/elasticache/developer-resources/
- type: x-testimonials
  url: https://aws.amazon.com/elasticache/testimonials/
- type: x-website
  url: https://aws.amazon.com/elasticache/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---