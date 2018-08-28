---
swagger: "2.0"
x-collection-name: Google Cloud Storage
x-complete: 0
info:
  title: Google Cloud Storage Get Objects
  version: 1.0.0
  description: Retrieves a list of objects matching the criteria.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /b/{bucket}/o:
    get:
      summary: Get Objects
      description: Retrieves a list of objects matching the criteria.
      operationId: storage.objects.list
      x-api-path-slug: bbucketo-get
      parameters:
      - in: path
        name: bucket
        description: Name of the bucket in which to look for objects
      - in: query
        name: delimiter
        description: Returns results in a directory-like mode
      - in: query
        name: maxResults
        description: Maximum number of items plus prefixes to return in a single page
          of responses
      - in: query
        name: pageToken
        description: A previously-returned page token representing part of the larger
          set of results to view
      - in: query
        name: prefix
        description: Filter results to objects whose names begin with this prefix
      - in: query
        name: projection
        description: Set of properties to return
      - in: query
        name: versions
        description: If true, lists all versions of an object as distinct results
      responses:
        200:
          description: OK
      tags:
      - Object
    post:
      summary: Add New Object
      description: Stores a new object and metadata.
      operationId: storage.objects.insert
      x-api-path-slug: bbucketo-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of the bucket in which to store the new object
      - in: query
        name: contentEncoding
        description: If set, sets the contentEncoding property of the final object
          to this value
      - in: query
        name: ifGenerationMatch
        description: Makes the operation conditional on whether the objects current
          generation matches the given value
      - in: query
        name: ifGenerationNotMatch
        description: Makes the operation conditional on whether the objects current
          generation does not match the given value
      - in: query
        name: ifMetagenerationMatch
        description: Makes the operation conditional on whether the objects current
          metageneration matches the given value
      - in: query
        name: ifMetagenerationNotMatch
        description: Makes the operation conditional on whether the objects current
          metageneration does not match the given value
      - in: query
        name: name
        description: Name of the object
      - in: query
        name: predefinedAcl
        description: Apply a predefined set of access controls to this object
      - in: query
        name: projection
        description: Set of properties to return
      responses:
        200:
          description: OK
      tags:
      - Object
  /b/{bucket}/o/watch:
    post:
      summary: Update Object
      description: Watch for changes on all objects in a bucket.
      operationId: storage.objects.watchAll
      x-api-path-slug: bbucketowatch-post
      parameters:
      - in: path
        name: bucket
        description: Name of the bucket in which to look for objects
      - in: query
        name: delimiter
        description: Returns results in a directory-like mode
      - in: query
        name: maxResults
        description: Maximum number of items plus prefixes to return in a single page
          of responses
      - in: query
        name: pageToken
        description: A previously-returned page token representing part of the larger
          set of results to view
      - in: query
        name: prefix
        description: Filter results to objects whose names begin with this prefix
      - in: query
        name: projection
        description: Set of properties to return
      - in: body
        name: resource
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: versions
        description: If true, lists all versions of an object as distinct results
      responses:
        200:
          description: OK
      tags:
      - Object
  /b/{bucket}/o/{object}:
    delete:
      summary: Delete Object
      description: Deletes an object and its metadata. Deletions are permanent if
        versioning is not enabled for the bucket, or if the generation parameter is
        used.
      operationId: storage.objects.delete
      x-api-path-slug: bbucketoobject-delete
      parameters:
      - in: path
        name: bucket
        description: Name of the bucket in which the object resides
      - in: query
        name: generation
        description: If present, permanently deletes a specific revision of this object
          (as opposed to the latest version, the default)
      - in: query
        name: ifGenerationMatch
        description: Makes the operation conditional on whether the objects current
          generation matches the given value
      - in: query
        name: ifGenerationNotMatch
        description: Makes the operation conditional on whether the objects current
          generation does not match the given value
      - in: query
        name: ifMetagenerationMatch
        description: Makes the operation conditional on whether the objects current
          metageneration matches the given value
      - in: query
        name: ifMetagenerationNotMatch
        description: Makes the operation conditional on whether the objects current
          metageneration does not match the given value
      - in: path
        name: object
        description: Name of the object
      responses:
        200:
          description: OK
      tags:
      - Object
    get:
      summary: Get Object
      description: Retrieves an object or its metadata.
      operationId: storage.objects.get
      x-api-path-slug: bbucketoobject-get
      parameters:
      - in: path
        name: bucket
        description: Name of the bucket in which the object resides
      - in: query
        name: generation
        description: If present, selects a specific revision of this object (as opposed
          to the latest version, the default)
      - in: query
        name: ifGenerationMatch
        description: Makes the operation conditional on whether the objects generation
          matches the given value
      - in: query
        name: ifGenerationNotMatch
        description: Makes the operation conditional on whether the objects generation
          does not match the given value
      - in: query
        name: ifMetagenerationMatch
        description: Makes the operation conditional on whether the objects current
          metageneration matches the given value
      - in: query
        name: ifMetagenerationNotMatch
        description: Makes the operation conditional on whether the objects current
          metageneration does not match the given value
      - in: path
        name: object
        description: Name of the object
      - in: query
        name: projection
        description: Set of properties to return
      responses:
        200:
          description: OK
      tags:
      - Object
    patch:
      summary: Update Object
      description: Updates an object's metadata. This method supports patch semantics.
      operationId: storage.objects.patch
      x-api-path-slug: bbucketoobject-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of the bucket in which the object resides
      - in: query
        name: generation
        description: If present, selects a specific revision of this object (as opposed
          to the latest version, the default)
      - in: query
        name: ifGenerationMatch
        description: Makes the operation conditional on whether the objects current
          generation matches the given value
      - in: query
        name: ifGenerationNotMatch
        description: Makes the operation conditional on whether the objects current
          generation does not match the given value
      - in: query
        name: ifMetagenerationMatch
        description: Makes the operation conditional on whether the objects current
          metageneration matches the given value
      - in: query
        name: ifMetagenerationNotMatch
        description: Makes the operation conditional on whether the objects current
          metageneration does not match the given value
      - in: path
        name: object
        description: Name of the object
      - in: query
        name: predefinedAcl
        description: Apply a predefined set of access controls to this object
      - in: query
        name: projection
        description: Set of properties to return
      responses:
        200:
          description: OK
      tags:
      - Object
    put:
      summary: Update Object
      description: Updates an object's metadata.
      operationId: storage.objects.update
      x-api-path-slug: bbucketoobject-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of the bucket in which the object resides
      - in: query
        name: generation
        description: If present, selects a specific revision of this object (as opposed
          to the latest version, the default)
      - in: query
        name: ifGenerationMatch
        description: Makes the operation conditional on whether the objects current
          generation matches the given value
      - in: query
        name: ifGenerationNotMatch
        description: Makes the operation conditional on whether the objects current
          generation does not match the given value
      - in: query
        name: ifMetagenerationMatch
        description: Makes the operation conditional on whether the objects current
          metageneration matches the given value
      - in: query
        name: ifMetagenerationNotMatch
        description: Makes the operation conditional on whether the objects current
          metageneration does not match the given value
      - in: path
        name: object
        description: Name of the object
      - in: query
        name: predefinedAcl
        description: Apply a predefined set of access controls to this object
      - in: query
        name: projection
        description: Set of properties to return
      responses:
        200:
          description: OK
      tags:
      - Object
  /b/{destinationBucket}/o/{destinationObject}/compose:
    post:
      summary: Concatenate Objects
      description: Concatenates a list of existing objects into a new object in the
        same bucket.
      operationId: storage.objects.compose
      x-api-path-slug: bdestinationbucketodestinationobjectcompose-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: destinationBucket
        description: Name of the bucket in which to store the new object
      - in: path
        name: destinationObject
        description: Name of the new object
      - in: query
        name: destinationPredefinedAcl
        description: Apply a predefined set of access controls to the destination
          object
      - in: query
        name: ifGenerationMatch
        description: Makes the operation conditional on whether the objects current
          generation matches the given value
      - in: query
        name: ifMetagenerationMatch
        description: Makes the operation conditional on whether the objects current
          metageneration matches the given value
      responses:
        200:
          description: OK
      tags:
      - Object
  /b/{sourceBucket}/o/{sourceObject}/copyTo/b/{destinationBucket}/o/{destinationObject}:
    post:
      summary: Copy Object
      description: Copies a source object to a destination object. Optionally overrides
        metadata.
      operationId: storage.objects.copy
      x-api-path-slug: bsourcebucketosourceobjectcopytobdestinationbucketodestinationobject-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: destinationBucket
        description: Name of the bucket in which to store the new object
      - in: path
        name: destinationObject
        description: Name of the new object
      - in: query
        name: destinationPredefinedAcl
        description: Apply a predefined set of access controls to the destination
          object
      - in: query
        name: ifGenerationMatch
        description: Makes the operation conditional on whether the destination objects
          current generation matches the given value
      - in: query
        name: ifGenerationNotMatch
        description: Makes the operation conditional on whether the destination objects
          current generation does not match the given value
      - in: query
        name: ifMetagenerationMatch
        description: Makes the operation conditional on whether the destination objects
          current metageneration matches the given value
      - in: query
        name: ifMetagenerationNotMatch
        description: Makes the operation conditional on whether the destination objects
          current metageneration does not match the given value
      - in: query
        name: ifSourceGenerationMatch
        description: Makes the operation conditional on whether the source objects
          generation matches the given value
      - in: query
        name: ifSourceGenerationNotMatch
        description: Makes the operation conditional on whether the source objects
          generation does not match the given value
      - in: query
        name: ifSourceMetagenerationMatch
        description: Makes the operation conditional on whether the source objects
          current metageneration matches the given value
      - in: query
        name: ifSourceMetagenerationNotMatch
        description: Makes the operation conditional on whether the source objects
          current metageneration does not match the given value
      - in: query
        name: projection
        description: Set of properties to return
      - in: path
        name: sourceBucket
        description: Name of the bucket in which to find the source object
      - in: query
        name: sourceGeneration
        description: If present, selects a specific revision of the source object
          (as opposed to the latest version, the default)
      - in: path
        name: sourceObject
        description: Name of the source object
      responses:
        200:
          description: OK
      tags:
      - Object
  /b/{sourceBucket}/o/{sourceObject}/rewriteTo/b/{destinationBucket}/o/{destinationObject}:
    post:
      summary: Rewrite Object
      description: Rewrites a source object to a destination object. Optionally overrides
        metadata.
      operationId: storage.objects.rewrite
      x-api-path-slug: bsourcebucketosourceobjectrewritetobdestinationbucketodestinationobject-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: destinationBucket
        description: Name of the bucket in which to store the new object
      - in: path
        name: destinationObject
        description: Name of the new object
      - in: query
        name: destinationPredefinedAcl
        description: Apply a predefined set of access controls to the destination
          object
      - in: query
        name: ifGenerationMatch
        description: Makes the operation conditional on whether the destination objects
          current generation matches the given value
      - in: query
        name: ifGenerationNotMatch
        description: Makes the operation conditional on whether the destination objects
          current generation does not match the given value
      - in: query
        name: ifMetagenerationMatch
        description: Makes the operation conditional on whether the destination objects
          current metageneration matches the given value
      - in: query
        name: ifMetagenerationNotMatch
        description: Makes the operation conditional on whether the destination objects
          current metageneration does not match the given value
      - in: query
        name: ifSourceGenerationMatch
        description: Makes the operation conditional on whether the source objects
          generation matches the given value
      - in: query
        name: ifSourceGenerationNotMatch
        description: Makes the operation conditional on whether the source objects
          generation does not match the given value
      - in: query
        name: ifSourceMetagenerationMatch
        description: Makes the operation conditional on whether the source objects
          current metageneration matches the given value
      - in: query
        name: ifSourceMetagenerationNotMatch
        description: Makes the operation conditional on whether the source objects
          current metageneration does not match the given value
      - in: query
        name: maxBytesRewrittenPerCall
        description: The maximum number of bytes that will be rewritten per rewrite
          request
      - in: query
        name: projection
        description: Set of properties to return
      - in: query
        name: rewriteToken
        description: Include this field (from the previous rewrite response) on each
          rewrite request after the first one, until the rewrite response done flag
          is true
      - in: path
        name: sourceBucket
        description: Name of the bucket in which to find the source object
      - in: query
        name: sourceGeneration
        description: If present, selects a specific revision of the source object
          (as opposed to the latest version, the default)
      - in: path
        name: sourceObject
        description: Name of the source object
      responses:
        200:
          description: OK
      tags:
      - Object
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