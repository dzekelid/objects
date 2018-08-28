---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Retrieves a list of objects stored in the cache system by its {listKey}
  version: 1.0.0
  description: Retrieves a list of objects stored in the cache system by its {listkey}.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/cache/List/{listKey}:
    get:
      summary: Retrieves a list of objects stored in the cache system by its {listKey}
      description: Retrieves a list of objects stored in the cache system by its {listkey}.
      operationId: Cache_GetListBylistKey
      x-api-path-slug: apicachelistlistkey-get
      parameters:
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Retrieves
      - List
      - Of
      - Objects
      - Stored
      - In
      - Cache
      - System
      - By
      - Its
      - ListKey
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