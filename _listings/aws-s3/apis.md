---
name: AWS S3
x-slug: aws-s3
description: Amazon Simple Storage Service (Amazon S3) is object storage with a simple
  web service interface to store and retrieve any amount of data from anywhere on
  the web. It is designed to deliver 99.999999999% durability, and scale past trillions
  of objects worldwide.Customers use S3 as a bulk repository, or data lake, for analytics;
  backup &amp; recovery; disaster recovery; and serverless computing. Many cloud-native
  applications even use S3 as primary storage.Its simple to move large volumes of
  data into or out of S3 with Amazonscloud data migrationoptions. Once data is stored
  in Amazon S3, it can be automatically tiered into lower cost, longer-termcloud storageclasses
  like S3 Standard - Infrequent Access and Amazon Glacier for archiving.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Objects
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/apis.md
specificationVersion: "0.14"
apis:
- name: No Title - Delete Multiple Objects
  x-api-slug: delete-post
  description: The Multi-Object Delete operation enables you to delete multiple objects
    from a bucketusing a single HTTP request
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/delete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/delete-post-openapi.md
- name: No Title - GET Bucket (List Objects) Version 2
  x-api-slug: listtype2-get
  description: This implementation of the GET operation returns some or all (up to
    1,000) ofthe objects in a bucket
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/listtype2-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/listtype2-get-openapi.md
- name: No Title - POST Object
  x-api-slug: post
  description: The POST operation adds an object to a specified bucket using HTML
    forms
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/post-openapi.md
- name: No Title - GET Bucket Object versions
  x-api-slug: versions-get
  description: You can use the versions subresource to list metadata about all ofthe
    versions of objects in a bucket
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/versions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/versions-get-openapi.md
- name: No Title - PUT Object - Copy
  x-api-slug: destinationobject-put
  description: This implementation of the PUT operation creates a copy of an object
    that is      already stored in Amazon S3
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/destinationobject-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/destinationobject-put-openapi.md
- name: No Title - DELETE Object
  x-api-slug: objectname-delete
  description: The DELETE operation removes the null version (if there is one) of
    anobject and inserts a delete marker, which becomes the current version of the
    object
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-delete-openapi.md
- name: No Title - GET Object
  x-api-slug: objectname-get
  description: This implementation of the GET operation retrieves objects from Amazon
    S3
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-get-openapi.md
- name: No Title - HEAD Object
  x-api-slug: objectname-head
  description: The HEAD operation retrieves metadata from an object without returning
    theobject itself
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-head-openapi.md
- name: No Title - OPTIONS object
  x-api-slug: objectname-options
  description: A browser can send this preflight request to Amazon S3 to determine
    if it can send an actualrequest with the specific origin, HTTP method, and headers
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-options-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-options-openapi.md
- name: No Title - PUT Object
  x-api-slug: objectname-put
  description: This implementation of the PUT operation adds an object to a bucket
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-put-openapi.md
- name: No Title - GET Object ACL
  x-api-slug: objectnameacl-get
  description: This implementation of the GET operation uses the aclsubresource to
    return the access control list (ACL) of an object
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnameacl-get-openapi.md
- name: No Title - PUT Object ACL
  x-api-slug: objectnameacl-put
  description: This implementation of the PUT operation uses the aclsubresource to
    set the access control list (ACL) permissions for an object that alreadyexists
    in a bucket
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnameacl-put-openapi.md
- name: No Title - POST Object restore
  x-api-slug: objectnamerestoreampversionidversionid-post
  description: Restores a temporary copy of an archived object
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnamerestoreampversionidversionid-post-openapi.md
- name: No Title - GET Object tagging
  x-api-slug: objectnametagging-get
  description: This implementation of the GET operation returns the tags associated
    with anobject
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnametagging-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnametagging-get-openapi.md
- name: No Title - PUT Object tagging
  x-api-slug: objectnametagging-put
  description: This implementation of the PUT operation uses the taggingsubresource
    to add a set of tags to an existing object
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnametagging-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnametagging-put-openapi.md
- name: No Title - GET Object torrent
  x-api-slug: objectnametorrent-get
  description: This implementation of the GET operation uses thetorrent subresource
    to return torrent files from a bucket
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnametorrent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnametorrent-get-openapi.md
- name: No Title - DELETE Object tagging
  x-api-slug: objectkeytagging-delete
  description: This implementation of the DELETE operation uses thetagging subresource
    to remove the entire tag set from thespecified object
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectkeytagging-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectkeytagging-delete-openapi.md
- name: No Title - Delete Multiple Objects
  x-api-slug: delete-post
  description: The Multi-Object Delete operation enables you to delete multiple objects
    from a bucketusing a single HTTP request
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/delete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/delete-post-openapi.md
- name: No Title - GET Bucket (List Objects) Version 2
  x-api-slug: listtype2-get
  description: This implementation of the GET operation returns some or all (up to
    1,000) ofthe objects in a bucket
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/listtype2-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/listtype2-get-openapi.md
- name: No Title - POST Object
  x-api-slug: post
  description: The POST operation adds an object to a specified bucket using HTML
    forms
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/post-openapi.md
- name: No Title - DELETE Object tagging
  x-api-slug: objectkeytagging-delete
  description: This implementation of the DELETE operation uses thetagging subresource
    to remove the entire tag set from thespecified object
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectkeytagging-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectkeytagging-delete-openapi.md
- name: No Title - DELETE Object tagging
  x-api-slug: objectkeytagging-delete
  description: This implementation of the DELETE operation uses thetagging subresource
    to remove the entire tag set from thespecified object
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectkeytagging-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectkeytagging-delete-openapi.md
- name: No Title - GET Object torrent
  x-api-slug: objectnametorrent-get
  description: This implementation of the GET operation uses thetorrent subresource
    to return torrent files from a bucket
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnametorrent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnametorrent-get-openapi.md
- name: No Title - GET Object torrent
  x-api-slug: objectnametorrent-get
  description: This implementation of the GET operation uses thetorrent subresource
    to return torrent files from a bucket
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnametorrent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnametorrent-get-openapi.md
- name: No Title - PUT Object tagging
  x-api-slug: objectnametagging-put
  description: This implementation of the PUT operation uses the taggingsubresource
    to add a set of tags to an existing object
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnametagging-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnametagging-put-openapi.md
- name: No Title - PUT Object tagging
  x-api-slug: objectnametagging-put
  description: This implementation of the PUT operation uses the taggingsubresource
    to add a set of tags to an existing object
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnametagging-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnametagging-put-openapi.md
- name: No Title - GET Object tagging
  x-api-slug: objectnametagging-get
  description: This implementation of the GET operation returns the tags associated
    with anobject
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnametagging-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnametagging-get-openapi.md
- name: No Title - GET Object tagging
  x-api-slug: objectnametagging-get
  description: This implementation of the GET operation returns the tags associated
    with anobject
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnametagging-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnametagging-get-openapi.md
- name: No Title - POST Object restore
  x-api-slug: objectnamerestoreampversionidversionid-post
  description: Restores a temporary copy of an archived object
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnamerestoreampversionidversionid-post-openapi.md
- name: No Title - POST Object restore
  x-api-slug: objectnamerestoreampversionidversionid-post
  description: Restores a temporary copy of an archived object
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnamerestoreampversionidversionid-post-openapi.md
- name: No Title - PUT Object ACL
  x-api-slug: objectnameacl-put
  description: This implementation of the PUT operation uses the aclsubresource to
    set the access control list (ACL) permissions for an object that alreadyexists
    in a bucket
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnameacl-put-openapi.md
- name: No Title - PUT Object ACL
  x-api-slug: objectnameacl-put
  description: This implementation of the PUT operation uses the aclsubresource to
    set the access control list (ACL) permissions for an object that alreadyexists
    in a bucket
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnameacl-put-openapi.md
- name: No Title - GET Object ACL
  x-api-slug: objectnameacl-get
  description: This implementation of the GET operation uses the aclsubresource to
    return the access control list (ACL) of an object
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnameacl-get-openapi.md
- name: No Title - GET Object ACL
  x-api-slug: objectnameacl-get
  description: This implementation of the GET operation uses the aclsubresource to
    return the access control list (ACL) of an object
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectnameacl-get-openapi.md
- name: No Title - PUT Object
  x-api-slug: objectname-put
  description: This implementation of the PUT operation adds an object to a bucket
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-put-openapi.md
- name: No Title - PUT Object
  x-api-slug: objectname-put
  description: This implementation of the PUT operation adds an object to a bucket
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-put-openapi.md
- name: No Title - OPTIONS object
  x-api-slug: objectname-options
  description: A browser can send this preflight request to Amazon S3 to determine
    if it can send an actualrequest with the specific origin, HTTP method, and headers
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-options-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-options-openapi.md
- name: No Title - OPTIONS object
  x-api-slug: objectname-options
  description: A browser can send this preflight request to Amazon S3 to determine
    if it can send an actualrequest with the specific origin, HTTP method, and headers
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-options-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-options-openapi.md
- name: No Title - HEAD Object
  x-api-slug: objectname-head
  description: The HEAD operation retrieves metadata from an object without returning
    theobject itself
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-head-openapi.md
- name: No Title - HEAD Object
  x-api-slug: objectname-head
  description: The HEAD operation retrieves metadata from an object without returning
    theobject itself
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-head-openapi.md
- name: No Title - GET Object
  x-api-slug: objectname-get
  description: This implementation of the GET operation retrieves objects from Amazon
    S3
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-get-openapi.md
- name: No Title - GET Object
  x-api-slug: objectname-get
  description: This implementation of the GET operation retrieves objects from Amazon
    S3
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-get-openapi.md
- name: No Title - DELETE Object
  x-api-slug: objectname-delete
  description: The DELETE operation removes the null version (if there is one) of
    anobject and inserts a delete marker, which becomes the current version of the
    object
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-delete-openapi.md
- name: No Title - DELETE Object
  x-api-slug: objectname-delete
  description: The DELETE operation removes the null version (if there is one) of
    anobject and inserts a delete marker, which becomes the current version of the
    object
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/objectname-delete-openapi.md
- name: No Title - PUT Object - Copy
  x-api-slug: destinationobject-put
  description: This implementation of the PUT operation creates a copy of an object
    that is      already stored in Amazon S3
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/destinationobject-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/destinationobject-put-openapi.md
- name: No Title - PUT Object - Copy
  x-api-slug: destinationobject-put
  description: This implementation of the PUT operation creates a copy of an object
    that is      already stored in Amazon S3
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/destinationobject-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/destinationobject-put-openapi.md
- name: No Title - GET Bucket Object versions
  x-api-slug: versions-get
  description: You can use the versions subresource to list metadata about all ofthe
    versions of objects in a bucket
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/versions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/versions-get-openapi.md
- name: No Title - GET Bucket Object versions
  x-api-slug: versions-get
  description: You can use the versions subresource to list metadata about all ofthe
    versions of objects in a bucket
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonS3.png
  humanURL: https://aws.amazon.com/s3/
  baseURL: https:////
  tags: Amazon Web Services, Storage, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/versions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/aws-s3/versions-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.route.53.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.s3.stack.network
- type: x-documentation
  url: http://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/s3/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/s3/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/s3/pricing/
- type: x-sla
  url: https://aws.amazon.com/s3/sla/
- type: x-website
  url: https://aws.amazon.com/s3/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---