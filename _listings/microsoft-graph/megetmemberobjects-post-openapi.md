---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Get Member Objects
  description: Get member objects Returns all the groups and directory roles that
    a user, group, or directory object is a member of. This function is transitive.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/getMemberObjects:
    post:
      summary: Get Member Objects
      description: Get member objects Returns all the groups and directory roles that
        a user, group, or directory object is a member of. This function is transitive.
      operationId: GetMemberObjects
      x-api-path-slug: megetmemberobjects-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        type: application/json
      responses:
        200:
          description: OK
      tags:
      - Member
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