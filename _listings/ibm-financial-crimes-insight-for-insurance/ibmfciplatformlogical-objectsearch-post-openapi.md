---
swagger: "2.0"
x-collection-name: IBM Financial Crimes Insight for Insurance
x-complete: 0
info:
  title: IBM Financial Crimes Insight for Insurance API Retrieve business objects
    using the specified parameters
  description: "This method provides searches for business objects within the database.
    \ The results for searching on a time stamp field are affected by the way that
    DB2\xC2\xAE handles time stamps. The JSON string uses ISO format for time stamps,
    such as 2016-06-15T20:11:19.326-04:00. DB2 converts this value to 2016-06-15-20.11.19.326000.
    Because DB2 might add more precision by storing a time stamp as 2016-06-15-20.11.19.326nnnn,
    the search results might not return what is expected. Refer to your DB2 documentation
    for more information on time stamps."
  version: 1.0.0
host: fcihost.ibm.com:9443
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ibm/fci/platform/fact/entity/match:
    get:
      summary: Get a list of resolved objects from resolved entities for a given object.
      description: Get a list of resolved objects from resolved entities for a given
        object. Using the provided object ID, produce a list of all objects of the
        same business object type that have been determined to be 'matches'.
      operationId: getMatchedEntity
      x-api-path-slug: ibmfciplatformfactentitymatch-get
      parameters:
      - in: query
        name: count
        description: Number of objects to return; all if not included
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: query
        name: id
        description: Object id of the object
      - in: query
        name: logicalType
        description: Metadata element ID for a business object
      - in: query
        name: returnFlag
        description: Default value == 2
      - in: query
        name: threshold
        description: Minimum matching score to include a resolved entity; defaults
          to system property if not supplied
      - in: query
        name: type
        description: Stereotype for object
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Resolved
      - Objects
      - From
      - Resolved
      - Entitiesa
      - Given
      - Object
  /ibm/fci/platform/logical_object/search:
    post:
      summary: Retrieve business objects using the specified parameters
      description: "This method provides searches for business objects within the
        database.  The results for searching on a time stamp field are affected by
        the way that DB2\xC2\xAE handles time stamps. The JSON string uses ISO format
        for time stamps, such as 2016-06-15T20:11:19.326-04:00. DB2 converts this
        value to 2016-06-15-20.11.19.326000. Because DB2 might add more precision
        by storing a time stamp as 2016-06-15-20.11.19.326nnnn, the search results
        might not return what is expected. Refer to your DB2 documentation for more
        information on time stamps."
      operationId: searchInstanceData
      x-api-path-slug: ibmfciplatformlogical-objectsearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: query
        name: lob_type
        description: A valid business object type
      - in: query
        name: prominence
        description: Prominence level of the fields that you want returned
      - in: query
        name: rec_count
        description: The number of matching records to return
      - in: query
        name: start_idx
        description: The starting index of the matching records to return
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Business
      - Objects
      - Using
      - Specified
      - Parameters
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