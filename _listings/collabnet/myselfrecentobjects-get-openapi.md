---
swagger: "2.0"
x-collection-name: CollabNet
x-complete: 0
info:
  title: CollabNet TeamForge API Documentation Gets recent object list for the current
    user
  version: 1.0.0
  description: Gets recent object list for the current user.
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /objects/{objectid}/delivery:
    get:
      summary: Gets delivery information for the given object
      description: Gets delivery information for the given object.
      operationId: getObjectDeliveryInfo
      x-api-path-slug: objectsobjectiddelivery-get
      parameters:
      - in: path
        name: objectid
        description: Object id(commit or artifact)
      responses:
        200:
          description: OK
      tags:
      - Delivery
      - Informationthe
      - Given
      - Object
  /objects/{objectid}/comments:
    post:
      summary: Posts a comment on the given object id
      description: Posts a comment on the given object id.
      operationId: postComment
      x-api-path-slug: objectsobjectidcomments-post
      parameters:
      - in: body
        name: body
        description: Comment
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: objectid
        description: Object id
      responses:
        200:
          description: OK
      tags:
      - Comment
      - "On"
      - Given
      - Object
    get:
      summary: Gets the comments on the given object id
      description: Gets the comments on the given object id.
      operationId: getObjectComments
      x-api-path-slug: objectsobjectidcomments-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: path
        name: objectid
        description: Object id
      - in: query
        name: offset
        description: Offset
      - in: query
        name: sortby
        description: Sort by column name
      responses:
        200:
          description: OK
      tags:
      - Comments
      - "On"
      - Given
      - Object
  /objects/{objectid}/auditlog:
    get:
      summary: Gets a collection of audit transactions performed on the specified
        TeamForge object
      description: Gets a collection of audit transactions performed on the specified
        teamforge object.
      operationId: getAuditLog
      x-api-path-slug: objectsobjectidauditlog-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: path
        name: objectid
        description: Object identifier
      - in: query
        name: offset
        description: Offset
      responses:
        200:
          description: OK
      tags:
      - Collection
      - Of
      - Audit
      - Transactions
      - Performed
      - "On"
      - Specified
      - TeamForge
      - Object
  /objects/{objectid}/associations:
    get:
      summary: Gets the association information for the given object id
      description: Gets the association information for the given object id.
      operationId: getObjectAssociations
      x-api-path-slug: objectsobjectidassociations-get
      parameters:
      - in: query
        name: depth
        description: Number of levels
      - in: query
        name: includeDependencies
        description: Include dependency associations (parent and child)
      - in: query
        name: includeEvents
        description: Include events
      - in: query
        name: includePhantoms
        description: Include phantom events
      - in: query
        name: limit
        description: Maximum number of generic associations for an object
      - in: path
        name: objectid
        description: Object/Activity id
      responses:
        200:
          description: OK
      tags:
      - Association
      - Informationthe
      - Given
      - Object
  /myself/recent/objects:
    get:
      summary: Gets recent object list for the current user
      description: Gets recent object list for the current user.
      operationId: getMyRecentObjects
      x-api-path-slug: myselfrecentobjects-get
      parameters:
      - in: query
        name: count
        description: Max
      responses:
        200:
          description: OK
      tags:
      - Recent
      - Object
      - Listthe
      - Current
      - User
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