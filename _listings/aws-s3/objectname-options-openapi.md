---
swagger: "2.0"
x-collection-name: AWS S3
x-complete: 0
info:
  title: AWS S3 OPTIONS object
  version: 1.0.0
  description: A browser can send this preflight request to Amazon S3 to determine
    if it can send an actualrequest with the specific origin, HTTP method, and headers
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?delete:
    post:
      summary: Delete Multiple Objects
      description: The Multi-Object Delete operation enables you to delete multiple
        objects from a bucketusing a single HTTP request
      operationId: delete-multiple-objects
      x-api-path-slug: delete-post
      parameters:
      - in: header
        name: Content-Length
        description: Length of the body according to RFC 2616
      - in: header
        name: Content-MD5
        description: The base64-encoded 128-bit MD5 digest of the data
      - in: header
        name: x-amz-mfa
        description: The value is the concatenation of the authentication devices
          serial number, a space,tttttttttand the value that is displayed on your
          authenticationtttttttttdevice
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Objects
  /?list-type=2:
    get:
      summary: GET Bucket (List Objects) Version 2
      description: This implementation of the GET operation returns some or all (up
        to 1,000) ofthe objects in a bucket
      operationId: get-bucket-list-objects-version-2
      x-api-path-slug: listtype2-get
      parameters:
      - in: query
        name: continuation-token
        description: When the Amazon S3 response to this API call is truncated (that
          is, IsTruncated responsetttttttttelement value is true), the response also
          includes thettttttttttNextContinuationToken element, the value of whichtttttttttyou
          can use in the next request as thettttttttttcontinuation-token to list the
          next settttttttttof objects
      - in: query
        name: delimiter
        description: A delimiter is a character you use to group keys
      - in: query
        name: encoding-type
        description: Requests Amazon S3 to encode the response and specifies the encoding
          method totttttttttuse
      - in: query
        name: fetch-owner
        description: By default, the API does not return the Owner information in
          the response
      - in: query
        name: list-type
        description: Version 2 of the API requires this parameter and you must set
          its value to 2
      - in: query
        name: max-keys
        description: Sets the maximum number of keys returned in the response body
      - in: query
        name: prefix
        description: Limits the response to keys that begin with the specifiedtttttttttprefix
      - in: query
        name: start-after
        description: If you want the API to return key names after a specifictttttttttobject
          key in your key space, you can add this parameter
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - (List
      - Objects)
      - Version
      - "2"
  /:
    post:
      summary: POST Object
      description: The POST operation adds an object to a specified bucket using HTML
        forms
      operationId: post-object
      x-api-path-slug: post
      responses:
        200:
          description: OK
      tags:
      - Object
  /?versions:
    get:
      summary: GET Bucket Object versions
      description: You can use the versions subresource to list metadata about all
        ofthe versions of objects in a bucket
      operationId: get-bucket-object-versions
      x-api-path-slug: versions-get
      parameters:
      - in: query
        name: delimiter
        description: A delimiter is a character that you specify to group keys
      - in: query
        name: encoding-type
        description: Requests Amazon S3 to encode the response and specifies the encoding
          method totttttttttuse
      - in: query
        name: key-marker
        description: Specifies the key in the bucket that you want to start listingtttttttttfrom
      - in: query
        name: max-keys
        description: Sets the maximum number of keys returned in the response body
      - in: query
        name: prefix
        description: Use this parameter to select only those keys that begin withtttttttttthe
          specified prefix
      - in: query
        name: version-id-marker
        description: Specifies the object version you want to start listing from
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Object
      - Versions
  /destinationObject:
    put:
      summary: PUT Object - Copy
      description: This implementation of the PUT operation creates a copy of an object
        that is      already stored in Amazon S3
      operationId: put-object--copy
      x-api-path-slug: destinationobject-put
      responses:
        200:
          description: OK
      tags:
      - Object
      - '-'
      - Copy
  /ObjectName:
    delete:
      summary: DELETE Object
      description: The DELETE operation removes the null version (if there is one)
        of anobject and inserts a delete marker, which becomes the current version
        of the object
      operationId: delete-object
      x-api-path-slug: objectname-delete
      parameters:
      - in: header
        name: x-amz-mfa
        description: The value is the concatenation of the authenticationtttttttttdevices
          serial number, a space, and the value displayed on yourtttttttttauthentication
          device
      responses:
        200:
          description: OK
      tags:
      - Object
    get:
      summary: GET Object
      description: This implementation of the GET operation retrieves objects from
        Amazon S3
      operationId: get-object
      x-api-path-slug: objectname-get
      parameters:
      - in: query
        name: response-cache-control
        description: Sets the Cache-Control header of the response
      - in: query
        name: response-content-disposition
        description: Sets the Content-Disposition header of thetttttttttresponse
      - in: query
        name: response-content-encoding
        description: Sets the Content-Encoding header of the response
      - in: query
        name: response-content-language
        description: Sets the Content-Language header of thetttttttttresponse
      - in: query
        name: response-content-type
        description: Sets the Content-Type header of thetttttttttresponse
      - in: query
        name: response-expires
        description: Sets the Expires header of the response
      responses:
        200:
          description: OK
      tags:
      - Object
    head:
      summary: HEAD Object
      description: The HEAD operation retrieves metadata from an object without returning
        theobject itself
      operationId: head-object
      x-api-path-slug: objectname-head
      parameters:
      - in: header
        name: If-Match
        description: Return the object only if its entity tag (ETag) is the same as
          the one specified; otherwise, return a 412 (precondition failed)
      - in: header
        name: If-Modified-Since
        description: Return the object only if it has been modified since the specified
          time, otherwise return a 304 (not modified)
      - in: header
        name: If-None-Match
        description: Return the object only if its entity tag (ETag) is different
          from the one specified; otherwise, return a 304 (not modified)
      - in: header
        name: If-Unmodified-Since
        description: Return the object only if it has not been modified since the
          specified time, otherwise return a 412 (precondition failed)
      - in: header
        name: Range
        description: Downloads the specified range bytes of an object
      - in: header
        name: x-amz-server-side&#8203;-encryption&#8203;-customer-algorithm
        description: Specifies the algorithm to use to when decrypting the requested
          object
      - in: header
        name: x-amz-server-side&#8203;-encryption&#8203;-customer-key
        description: Specifies the customer-provided base64-encoded encryption key
          to use to decrypt the requested object
      - in: header
        name: x-amz-server-side&#8203;-encryption&#8203;-customer-key-MD5
        description: Specifies the base64-encoded 128-bit MD5 digest of the customer-provided
          encryption key according to ttttRFC 1321
      responses:
        200:
          description: OK
      tags:
      - Object
    options:
      summary: OPTIONS object
      description: A browser can send this preflight request to Amazon S3 to determine
        if it can send an actualrequest with the specific origin, HTTP method, and
        headers
      operationId: options-object
      x-api-path-slug: objectname-options
      responses:
        200:
          description: OK
      tags:
      - OPTIONS
      - Object
    put:
      summary: PUT Object
      description: This implementation of the PUT operation adds an object to a bucket
      operationId: put-object
      x-api-path-slug: objectname-put
      responses:
        200:
          description: OK
      tags:
      - Object
  /ObjectName?acl:
    get:
      summary: GET Object ACL
      description: This implementation of the GET operation uses the aclsubresource
        to return the access control list (ACL) of an object
      operationId: get-object-acl
      x-api-path-slug: objectnameacl-get
      responses:
        200:
          description: OK
      tags:
      - Object
      - ACL
    put:
      summary: PUT Object ACL
      description: This implementation of the PUT operation uses the aclsubresource
        to set the access control list (ACL) permissions for an object that alreadyexists
        in a bucket
      operationId: put-object-acl
      x-api-path-slug: objectnameacl-put
      parameters:
      - in: header
        name: x-amz-acl
        description: Sets the ACL of the object using the specified canned ACL
      - in: header
        name: x-amz-grant-full-control
        description: Allows the specified grantee the READ, WRITE, READ_ACP, andtttttttttWRITE_ACP
          permissions on the bucket
      - in: header
        name: x-amz-grant-read
        description: Allows the specified grantee to list the objects in thetttttttttbucket
      - in: header
        name: x-amz-grant-read-acp
        description: Allows the specified grantee to read the buckettttttttttACL
      - in: header
        name: x-amz-grant-write
        description: Not applicable when granting access permissions on objects
      - in: header
        name: x-amz-grant-write-acp
        description: Allows the specified grantee to write the ACL for thetttttttttapplicable
          bucket
      responses:
        200:
          description: OK
      tags:
      - Object
      - ACL
  /ObjectName?restore&amp;versionId=VersionID:
    post:
      summary: POST Object restore
      description: Restores a temporary copy of an archived object
      operationId: post-object-restore
      x-api-path-slug: objectnamerestoreampversionidversionid-post
      parameters:
      - in: header
        name: Content-MD5
        description: The base64-encoded 128-bit MD5 digest of the data
      responses:
        200:
          description: OK
      tags:
      - Object
      - Restore
  /ObjectName?tagging:
    get:
      summary: GET Object tagging
      description: This implementation of the GET operation returns the tags associated
        with anobject
      operationId: get-object-tagging
      x-api-path-slug: objectnametagging-get
      responses:
        200:
          description: OK
      tags:
      - Object
      - Tagging
    put:
      summary: PUT Object tagging
      description: This implementation of the PUT operation uses the taggingsubresource
        to add a set of tags to an existing object
      operationId: put-object-tagging
      x-api-path-slug: objectnametagging-put
      responses:
        200:
          description: OK
      tags:
      - Object
      - Tagging
  /ObjectName?torrent:
    get:
      summary: GET Object torrent
      description: This implementation of the GET operation uses thetorrent subresource
        to return torrent files from a bucket
      operationId: get-object-torrent
      x-api-path-slug: objectnametorrent-get
      responses:
        200:
          description: OK
      tags:
      - Object
      - Torrent
  ObjectKey/?tagging:
    delete:
      summary: DELETE Object tagging
      description: This implementation of the DELETE operation uses thetagging subresource
        to remove the entire tag set from thespecified object
      operationId: delete-object-tagging
      x-api-path-slug: objectkeytagging-delete
      responses:
        200:
          description: OK
      tags:
      - Object
      - Tagging
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