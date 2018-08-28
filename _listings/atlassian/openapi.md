swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
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