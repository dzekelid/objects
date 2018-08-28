---
swagger: "2.0"
x-collection-name: Neblio
x-complete: 0
info:
  title: Neblio Returns address object
  description: Returns NEBL address object containing information on a specific address
  version: 1.0.0
host: ntp1node.nebl.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ins/tx/{txid}:
    get:
      summary: Returns transaction object
      description: Returns NEBL transaction object representing a NEBL transaction
      operationId: getTx
      x-api-path-slug: instxtxid-get
      parameters:
      - in: path
        name: txid
        description: Transaction ID
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Transaction
      - Object
  /ins/addr/{address}:
    get:
      summary: Returns address object
      description: Returns NEBL address object containing information on a specific
        address
      operationId: getAddress
      x-api-path-slug: insaddraddress-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Address
      - Object
  /testnet/ins/tx/{txid}:
    get:
      summary: Returns transaction object
      description: Returns NEBL transaction object representing a NEBL transaction
      operationId: testnet_getTx
      x-api-path-slug: testnetinstxtxid-get
      parameters:
      - in: path
        name: txid
        description: Transaction ID
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Transaction
      - Object
  /testnet/ins/addr/{address}:
    get:
      summary: Returns address object
      description: Returns NEBL address object containing information on a specific
        address
      operationId: testnet_getAddress
      x-api-path-slug: testnetinsaddraddress-get
      parameters:
      - in: path
        name: address
        description: Address
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Returns
      - Address
      - Object
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