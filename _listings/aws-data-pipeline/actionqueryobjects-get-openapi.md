---
swagger: "2.0"
x-collection-name: AWS Data Pipeline
x-complete: 0
info:
  title: AWS Data Pipeline API Query Objects
  version: 1.0.0
  description: Queries the specified pipeline for the names of objects that match
    the specified set of conditions.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeObjects:
    get:
      summary: Describe Objects
      description: Gets the object definitions for a set of objects associated with
        the pipeline.
      operationId: describeObjects
      x-api-path-slug: actiondescribeobjects-get
      parameters:
      - in: query
        name: evaluateExpressions
        description: Indicates whether any expressions in the object should be evaluated
          when the object descriptions are returned
        type: string
      - in: query
        name: marker
        description: The starting point for the results to be returned
        type: string
      - in: query
        name: objectIds
        description: The IDs of the pipeline objects that contain the definitions
          to be described
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline that contains the object definitions
        type: string
      responses:
        200:
          description: OK
      tags:
      - Objects
  /?Action=QueryObjects:
    get:
      summary: Query Objects
      description: Queries the specified pipeline for the names of objects that match
        the specified set of conditions.
      operationId: queryObjects
      x-api-path-slug: actionqueryobjects-get
      parameters:
      - in: query
        name: limit
        description: The maximum number of object names that QueryObjects will return
          in a single call
        type: string
      - in: query
        name: marker
        description: The starting point for the results to be returned
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      - in: query
        name: query
        description: The query that defines the objects to be returned
        type: string
      - in: query
        name: sphere
        description: Indicates whether the query applies to components or instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Objects
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