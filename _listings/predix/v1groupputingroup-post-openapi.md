---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Fingerprint of Things Object Tagging Service Put Object in Group
  description: Put Object in Group.
  contact:
    name: NEC
  version: 1.0.0
host: fingerprint-of-things-ga1-dast.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{collection}:
    get:
      summary: Gets all user-defined domain objects.
      description: |-
        This is a user-defined domain object collection.

        You can create your own custom domain objects, add properties to them, define relationships, and so on.
      operationId: getV1Collection
      x-api-path-slug: v1collection-get
      parameters:
      - in: path
        name: collection
        description: Name of the user-defined domain object collection
      - in: query
        name: fields
        description: Fields to be returned from each entity (comma separated)
      - in: query
        name: filter
        description: GEL query filter
      - in: query
        name: pageSize
        description: Limits the number of entities returned
      responses:
        200:
          description: Successful response
      tags:
      - S
      - ""
      - User-defined
      - Domain
      - Objects
    post:
      summary: Create one or more user-defined domain objects
      description: |-
        This is a user-defined domain object collection.

        You can create your own custom domain objects, add properties to them, define relationships, and so on.

        The following characters are not allowed in any attribute names: $ < > : | ( ) , = ! ? &
      operationId: postV1Collection
      x-api-path-slug: v1collection-post
      parameters:
      - in: body
        name: body
        description: Array of entities to create
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collection
        description: Name of the user-defined domain object collection
      responses:
        200:
          description: Successful response
      tags:
      - More
      - User-defined
      - Domain
      - Objects
  /v1/:
    get:
      summary: Get a listing of user-defined domain object collections
      description: Returns the names of all user-defined domain object collections
        with counts of domain objects contained.
      operationId: getV1
      x-api-path-slug: v1-get
      responses:
        200:
          description: Successful response
      tags:
      - Listing
      - Of
      - User-defined
      - Domain
      - Object
      - Collections
  /v1/{collection}/{id}:
    put:
      summary: Update a user-defined domain object
      description: |-
        This is a user-defined domain object collection.

        You can create your own custom domain objects, add properties to them, define relationships, and so on.

        The following characters are not allowed in any attribute names: $ < > : | ( ) , = ! ? &
      operationId: putV1Collection
      x-api-path-slug: v1collectionid-put
      parameters:
      - in: body
        name: body
        description: Array of one entity to create/update
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collection
        description: Name of the user-defined domain object collection
      - in: path
        name: id
        description: ID of the domain object to update
      responses:
        200:
          description: Successful response
      tags:
      - User-defined
      - Domain
      - Object
    patch:
      summary: Patch a user-defined domain object
      description: |-
        This is a user-defined domain object collection.

        You can create your own custom domain objects, add properties to them, define relationships, and so on.

        Update specific model using http PATCH requests. Request format should follow JSON PATCH format. Supported operations on each attribute are add, remove, replace, move, copy, test. Refer RFC link for more details on request format. https://tools.ietf.org/html/rfc6902
      operationId: patchV1Collection
      x-api-path-slug: v1collectionid-patch
      parameters:
      - in: body
        name: body
        description: 'Array of patch operations to apply to the domain object (see:
          https://tools'
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collection
        description: Name of the user-defined domain object collection
      - in: path
        name: id
        description: ID of the domain object to patch
      responses:
        200:
          description: Successful response
      tags:
      - User-defined
      - Domain
      - Object
    delete:
      summary: Delete a user-defined domain object
      description: |-
        This is a user-defined domain object collection.

        You can create your own custom domain objects, add properties to them, define relationships, and so on.
      operationId: deleteV1Collection
      x-api-path-slug: v1collectionid-delete
      parameters:
      - in: path
        name: collection
        description: Name of the user-defined domain object collection
      - in: path
        name: id
        description: ID of the domain object to delete
      responses:
        200:
          description: Successful response
      tags:
      - User-defined
      - Domain
      - Object
  /v1/system/audit:
    get:
      summary: Get domain object audit records.
      description: For detailed documentation of all available query options please
        refer to Predix Asset Documentation.
      operationId: getV1SystemAudit
      x-api-path-slug: v1systemaudit-get
      parameters:
      - in: query
        name: fields
        description: Fields to be returned from the entity (comma separated)
      responses:
        200:
          description: Successful response
      tags:
      - Domain
      - Object
      - Audit
      - Records
  /v1/object/listObjects:
    post:
      summary: List Registered Objects
      description: List registered Objects.
      operationId: reference
      x-api-path-slug: v1objectlistobjects-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - List
      - Registered
      - Objects
  /v1/object/preregisterObject:
    post:
      summary: Object Pre-Register
      description: Pre-register object with image.<br> Individual ID must be designated
        by user.
      operationId: userIssue
      x-api-path-slug: v1objectpreregisterobject-post
      parameters:
      - in: formData
        name: applyFlag
        description: '* DO NOT USE'
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: formData
        name: individualId
        description: Individual ID
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      - in: formData
        name: registImage
        description: 'Image data(Max file size: 5MByte)'
      responses:
        200:
          description: OK
      tags:
      - Object
      - Pre-Register
  /v1/object/preregisterObjectWithoutID:
    post:
      summary: Object Pre-Register without ID
      description: Pre-register object with image.<br> Individual ID will be issued
        from system.
      operationId: systemIssue
      x-api-path-slug: v1objectpreregisterobjectwithoutid-post
      parameters:
      - in: formData
        name: applyFlag
        description: '* DO NOT USE'
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      - in: formData
        name: registImage
        description: 'Image data(Max file size: 5MByte)'
      responses:
        200:
          description: OK
      tags:
      - Object
      - Pre-Register
      - Without
      - ID
  /v1/object/deleteRegisteredObject:
    post:
      summary: Delete Registered Object
      description: Delete registered object.
      operationId: deleteRegularRegistration
      x-api-path-slug: v1objectdeleteregisteredobject-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Registered
      - Object
  /v1/object/deletePreregisteredObject:
    post:
      summary: Delete Pre-Registered Object
      description: Delete pre-registered object.
      operationId: deleteTempRegistration
      x-api-path-slug: v1objectdeletepreregisteredobject-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Pre-Registered
      - Object
  /v1/group/putInGroup:
    post:
      summary: Put Object in Group
      description: Put Object in Group.
      operationId: joinGroup
      x-api-path-slug: v1groupputingroup-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Object
      - In
      - Group
  /v1/group/removeFromGroup:
    post:
      summary: Remove Object from Group
      description: Remove Object from Group.
      operationId: leaveGroup
      x-api-path-slug: v1groupremovefromgroup-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Object
      - From
      - Group
  /v1/object/registerObject:
    post:
      summary: Register Object
      description: Register Object. A registered object can be queried from Query
        APIs.
      operationId: apply
      x-api-path-slug: v1objectregisterobject-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Register
      - Object
  /v1/object/registerGroup:
    post:
      summary: Register Object per Group
      description: Register Object per Group. A registered object can be queried from
        Query APIs.
      operationId: groupApply
      x-api-path-slug: v1objectregistergroup-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Register
      - Object
      - Per
      - Group
  /v1/object/checkPreregisteredObject:
    post:
      summary: Check Pre-Registered Object
      description: Check a score of Pre-Registered Object.
      operationId: check
      x-api-path-slug: v1objectcheckpreregisteredobject-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: formData
        name: individualId
        description: Individual ID
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      - in: formData
        name: registImage
        description: 'Image data(Max file size: 5MByte)'
      responses:
        200:
          description: OK
      tags:
      - Check
      - Pre-Registered
      - Object
  /v1/query/queryByObject:
    post:
      summary: Query by Object
      description: Query image by object.
      operationId: dozicheck
      x-api-path-slug: v1queryquerybyobject-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: formData
        name: checkResultDisplayNumber
        description: 'Result display number: Specify number of verification result
          to retrieve'
      - in: formData
        name: idSpecificationFlag
        description: 'ID specification flag (0: Query with all registered objects
          , 1: Query with specified object by individual ID)'
      - in: formData
        name: individualId
        description: 'Individual ID: Use CSV form when specifying multiple IDs'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      - in: formData
        name: queryImage
        description: 'Query image data(Max file size: 5MByte)'
      responses:
        200:
          description: OK
      tags:
      - Query
      - By
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