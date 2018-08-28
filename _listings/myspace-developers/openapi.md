swagger: "2.0"
x-collection-name: MySpace Developers
x-complete: 1
info:
  title: My Space
  description: create-apps-and-games-within-the-myspace-platform--monetize-through-advertising-and-virtual-goods-
  version: 1.0.0
host: api.myspace.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /1.0/activities/@supportedObjectTypes:
    get:
      summary: Get Activities Supported Object Types
      description: Retrieves all supported object types.
      operationId: 1.0.activities._supportedObjectTypes.get
      x-api-path-slug: 1-0activitiessupportedobjecttypes-get
      parameters:
      - in: query
        name: count
        description: Only returns the nearest multiple of 3 compared to the original
          value
      - in: query
        name: fields
        description: The following field names are supported
      - in: query
        name: format
        description: Determines the format of the response
      - in: query
        name: startIndex
        description: Indicates the index of the first item to retrieve from the query
          set
      - in: query
        name: updatedSince
        description: Indicates the date before which no activities should be returned
      responses:
        200:
          description: OK
      tags:
      - Activities
      - Supported
      - ObjectTypes