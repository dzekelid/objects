---
swagger: "2.0"
info:
  title: SalesForce Get Version Sobjects
  description: Lists the available objects and their metadata for your organization's
    data. In addition, it provides the organization encoding, as well as maximum batch
    size permitted in queries. For more information, see Internationalization and
    Character Sets (http://www.salesforce.com/us/developer/docs/api/Content/implementation_considerations.htm#sforce_api_other_internationalization).
  version: 1.0.0
host: na14.salesforce.com
basePath: /services/data
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{version}/sobjects:
    get:
      summary: Get Version Sobjects
      description: Lists the available objects and their metadata for your organization's
        data
      operationId: version.sobjects.get
      responses:
        200:
          description: OK
      tags:
      - version
      - sobjects
definitions: []
x-collection-name: Salesforce
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