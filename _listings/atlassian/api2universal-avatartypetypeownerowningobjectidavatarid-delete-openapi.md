---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Delete avatar
  description: Deletes avatar
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/universal_avatar/type/{type}/owner/{owningObjectId}/avatar/{id}:
    delete:
      summary: Delete avatar
      description: Deletes avatar
      operationId: com.atlassian.jira.rest.v2.issue.UniversalAvatarResource.deleteAvatar_delete
      x-api-path-slug: api2universal-avatartypetypeownerowningobjectidavatarid-delete
      parameters:
      - in: path
        name: id
        description: database id for avatar
      - in: path
        name: owningObjectId
      - in: path
        name: type
        description: Project id or project key
      responses:
        200:
          description: OK
      tags:
      - Avatar
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