swagger: "2.0"
x-collection-name: IBM Financial Crimes Insight for Insurance
x-complete: 1
info:
  title: Financial Crimes Insight for Insurance public REST APIs
  description: these-are-the-financial-crimes-insight-for-insurance-public-rest-apis-used-by-clients-to-access-the-fcii-capabilities
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
  /ibm/fci/platform/fact/{type}/{remoteSystem}/{remoteKey}/assessments]:
    get:
      summary: Return the existing assessments for the object specified
      description: This service is used to return the existing assessments for the
        object specified.
      operationId: requestAssessmentValue
      x-api-path-slug: ibmfciplatformfacttyperemotesystemremotekeyassessments-get
      parameters:
      - in: query
        name: context
        description: The fraud context for which to return assessements
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: path
        name: remoteKey
        description: The combination of remoteSystem and remoteKey uniquely defines
          an object
      - in: path
        name: remoteSystem
        description: The combination of remoteSystem and remoteKey uniquely defines
          an object
      - in: path
        name: type
        description: Type of object; party, account, transaction, event, or other
          defined object type
      responses:
        200:
          description: OK
      tags:
      - Return
      - Existing
      - Assessmentsthe
      - Object
      - Specified
  /ibm/fci/platform/fact/match:
    get:
      summary: Determine if one object is a match to the other.
      description: Using the provided objects, determine if one is a 'match' of the
        other
      operationId: getMatchedObject
      x-api-path-slug: ibmfciplatformfactmatch-get
      parameters:
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: query
        name: objectId1
        description: Object id of first object
      - in: query
        name: objectId2
        description: Object id of second object
      - in: query
        name: objectStereotype
        description: stereotype of the objects being compared
      - in: query
        name: updateResolvedEntities
        description: Boolean to indicate whether or not to record relationship
      responses:
        200:
          description: OK
      tags:
      - Determine
      - If
      - Object
      - Is
      - Match
      - To
      - Other
  /ibm/fci/platform/fact/physical_object:
    put:
      summary: Insert physical object data into the database
      description: This method is used to insert physical object data into the database.  The
        XML schema is defined in the PhysicalObject.XSD file.
      operationId: putPhysicalObject
      x-api-path-slug: ibmfciplatformfactphysical-object-put
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
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Physical
      - Object
      - Data
      - Into
      - Database
  /ibm/fci/platform/fact/physical_object/{id}:
    get:
      summary: Retrieve a specific physical object data from the database, based on
        its internal id
      description: This method is used to retrieve specific physical object data from
        the database, based on its internal id
      operationId: getPhysicalObject
      x-api-path-slug: ibmfciplatformfactphysical-objectid-get
      parameters:
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Specific
      - Physical
      - Object
      - Data
      - From
      - Database
      - ""
      - Based
      - "On"
      - Its
      - Internal
      - Id