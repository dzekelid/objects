---
name: Google Cloud Storage
x-slug: google-cloud-storage
description: Google Cloud Storage is unified object storage for developers and enterprises,
  from live data serving to data analytics/ML to data archiving. Google Cloud Storage
  allows world-wide storage and retrieval of any amount of data at any time. You can
  use Google Cloud Storage for a range of scenarios including serving website content,
  storing data for archival and disaster recovery, or distributing large data objects
  to users via direct download.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Objects
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/apis.md
specificationVersion: "0.14"
apis:
- name: Google Cloud Storage - Get Objects
  x-api-slug: bbucketo-get
  description: Retrieves a list of objects matching the criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bbucketo-get-openapi.md
- name: Google Cloud Storage - Add New Object
  x-api-slug: bbucketo-post
  description: Stores a new object and metadata.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bbucketo-post-openapi.md
- name: Google Cloud Storage - Update Object
  x-api-slug: bbucketowatch-post
  description: Watch for changes on all objects in a bucket.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bbucketowatch-post-openapi.md
- name: Google Cloud Storage - Delete Object
  x-api-slug: bbucketoobject-delete
  description: Deletes an object and its metadata. Deletions are permanent if versioning
    is not enabled for the bucket, or if the generation parameter is used.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bbucketoobject-delete-openapi.md
- name: Google Cloud Storage - Get Object
  x-api-slug: bbucketoobject-get
  description: Retrieves an object or its metadata.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bbucketoobject-get-openapi.md
- name: Google Cloud Storage - Update Object
  x-api-slug: bbucketoobject-patch
  description: Updates an object's metadata. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bbucketoobject-patch-openapi.md
- name: Google Cloud Storage - Update Object
  x-api-slug: bbucketoobject-put
  description: Updates an object's metadata.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bbucketoobject-put-openapi.md
- name: Google Cloud Storage - Concatenate Objects
  x-api-slug: bdestinationbucketodestinationobjectcompose-post
  description: Concatenates a list of existing objects into a new object in the same
    bucket.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bdestinationbucketodestinationobjectcompose-post-openapi.md
- name: Google Cloud Storage - Copy Object
  x-api-slug: bsourcebucketosourceobjectcopytobdestinationbucketodestinationobject-post
  description: Copies a source object to a destination object. Optionally overrides
    metadata.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bsourcebucketosourceobjectcopytobdestinationbucketodestinationobject-post-openapi.md
- name: Google Cloud Storage - Rewrite Object
  x-api-slug: bsourcebucketosourceobjectrewritetobdestinationbucketodestinationobject-post
  description: Rewrites a source object to a destination object. Optionally overrides
    metadata.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bsourcebucketosourceobjectrewritetobdestinationbucketodestinationobject-post-openapi.md
- name: Google Cloud Storage - Rewrite Object
  x-api-slug: bsourcebucketosourceobjectrewritetobdestinationbucketodestinationobject-post
  description: Rewrites a source object to a destination object. Optionally overrides
    metadata.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bsourcebucketosourceobjectrewritetobdestinationbucketodestinationobject-post-openapi.md
- name: Google Cloud Storage - Copy Object
  x-api-slug: bsourcebucketosourceobjectcopytobdestinationbucketodestinationobject-post
  description: Copies a source object to a destination object. Optionally overrides
    metadata.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bsourcebucketosourceobjectcopytobdestinationbucketodestinationobject-post-openapi.md
- name: Google Cloud Storage - Concatenate Objects
  x-api-slug: bdestinationbucketodestinationobjectcompose-post
  description: Concatenates a list of existing objects into a new object in the same
    bucket.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bdestinationbucketodestinationobjectcompose-post-openapi.md
- name: Google Cloud Storage - Update Object
  x-api-slug: bbucketoobject-put
  description: Updates an object's metadata.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bbucketoobject-put-openapi.md
- name: Google Cloud Storage - Update Object
  x-api-slug: bbucketoobject-patch
  description: Updates an object's metadata. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bbucketoobject-patch-openapi.md
- name: Google Cloud Storage - Get Object
  x-api-slug: bbucketoobject-get
  description: Retrieves an object or its metadata.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bbucketoobject-get-openapi.md
- name: Google Cloud Storage - Delete Object
  x-api-slug: bbucketoobject-delete
  description: Deletes an object and its metadata. Deletions are permanent if versioning
    is not enabled for the bucket, or if the generation parameter is used.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bbucketoobject-delete-openapi.md
- name: Google Cloud Storage - Update Object
  x-api-slug: bbucketowatch-post
  description: Watch for changes on all objects in a bucket.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bbucketowatch-post-openapi.md
- name: Google Cloud Storage - Add New Object
  x-api-slug: bbucketo-post
  description: Stores a new object and metadata.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bbucketo-post-openapi.md
- name: Google Cloud Storage - Get Objects
  x-api-slug: bbucketo-get
  description: Retrieves a list of objects matching the criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-storage-unified-object-storage-2x.png
  humanURL: https://cloud.google.com/storage/
  baseURL: https:///
  tags: Google APIs, Cloud, Storage, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/google-cloud-storage/bbucketo-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.cloud.sql.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.cloud.storage.stack.network
- type: x-authentication
  url: https://cloud.google.com/storage/docs/authentication
- type: x-best-practices
  url: https://cloud.google.com/storage/docs/best-practices
- type: x-change-log
  url: https://cloud.google.com/storage/release-notes
- type: x-code
  url: https://cloud.google.com/storage/docs/reference/libraries
- type: x-concepts
  url: https://cloud.google.com/storage/docs/concepts
- type: x-dmca-policy
  url: https://cloud.google.com/storage/docs/dmca
- type: x-faq
  url: https://cloud.google.com/storage/docs/faq
- type: x-getting-started
  url: https://cloud.google.com/storage/docs/quickstarts
- type: x-guides
  url: https://cloud.google.com/storage/docs/how-to
- type: x-pricing
  url: https://cloud.google.com/storage/pricing
- type: x-service-level-agreements
  url: https://cloud.google.com/storage/sla
- type: x-support
  url: https://cloud.google.com/storage/docs/resources-support
- type: x-tutorials
  url: https://cloud.google.com/storage/docs/tutorials
- type: x-website
  url: https://cloud.google.com/storage/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---