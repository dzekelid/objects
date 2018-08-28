swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 1
info:
  title: GoToWebinar API
  description: todo-add-description
  version: 1.0.0
host: api.getgo.com
basePath: /G2W/rest/organizers
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:
    put:
      summary: Associate Ticket
      description: "Associates a ticket for a particular partner with a current session.\n\n
        \ Request Parameters:                  \n                    \n    field      data
        type      description    \n    sessionId      string      The unique ID of
        the session to associate with the new partner object.    \n    userToken      string
        \     The token identifying and authenticating the user in the partner system
        that this object is being created on behalf of this user.    \n    partnerObject
        \     string      The partner object to associate with the session."
      operationId: UnnammedEndpointPut
      x-api-path-slug: put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Associate
      - Ticket