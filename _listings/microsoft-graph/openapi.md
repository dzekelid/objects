swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
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
  /users/{id | userPrincipalName}/getMemberObjects:
    post:
      summary: Get Member Objects
      description: Get member objects Returns all the groups and directory roles that
        a user, group, or directory object is a member of. This function is transitive.
      operationId: GetMemberObjects
      x-api-path-slug: usersid--userprincipalnamegetmemberobjects-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Member
      - Objects
  /directoryObjects/{id}/getMemberObjects:
    post:
      summary: Get Member Objects
      description: Get member objects Returns all the groups and directory roles that
        a user, group, or directory object is a member of. This function is transitive.
      operationId: GetMemberObjects
      x-api-path-slug: directoryobjectsidgetmemberobjects-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        type: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Member
      - Objects
  /groups/{id}/getMemberObjects:
    post:
      summary: Group Get Member Objects
      description: 'group: getMemberObjects Return all of the groups that this group
        is a member of. The check is transitive. Note: Groups cannot be members of
        directory roles, so no directory roles will be returned.'
      operationId: Group:GetMemberObjects
      x-api-path-slug: groupsidgetmemberobjects-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - ""
      - Member
      - Objects
  /users/{id | userPrincipalName}/createdObjects:
    get:
      summary: List Created Objects
      description: List createdObjects Get a list of directory objects that were created
        by the user.
      operationId: ListCreatedObjects
      x-api-path-slug: usersid--userprincipalnamecreatedobjects-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Created
      - Objects
  /users/{id | userPrincipalName}/ownedObjects:
    get:
      summary: List Owned Objects
      description: List ownedObjects Get the list of directory objects that are owned
        by the user.
      operationId: ListOwnedObjects
      x-api-path-slug: usersid--userprincipalnameownedobjects-get
      parameters:
      - in: header
        name: Accept
        description: application/json
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Owned
      - Objects
  /directoryObjects/{id}:
    delete:
      summary: Delete Directory Object
      description: Delete directoryObject Deletes a directoryObject.
      operationId: DeleteDirectoryObject
      x-api-path-slug: directoryobjectsid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Directory
      - Object
    get:
      summary: Get Directory Object
      description: Get directoryObject Retrieve the properties and relationships of
        directoryObject object.
      operationId: GetDirectoryObject
      x-api-path-slug: directoryobjectsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Directory
      - Object