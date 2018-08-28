---
swagger: "2.0"
x-collection-name: Lisk
x-complete: 0
info:
  title: Lisk Submits a signature object to sign multisignature transactions
  description: |-
    Submits signature to sign a multisignature transaction.
    Signature objects can be generated locally either by using Lisk Commander or with Lisk Elements.
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /signatures:
    post:
      summary: Submits a signature object to sign multisignature transactions
      description: |-
        Submits signature to sign a multisignature transaction.
        Signature objects can be generated locally either by using Lisk Commander or with Lisk Elements.
      operationId: postSignature
      x-api-path-slug: signatures-post
      parameters:
      - in: body
        name: signature
        description: Signature object to submit to the network
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Submits
      - Signature
      - Object
      - To
      - Sign
      - Multisignature
      - Transactions
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