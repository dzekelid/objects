---
name: Salesforce Sandbox
x-slug: salesforce-sandbox
description: Quick and easy mock RESTful API and SOAP webservices. Generate from API
  definitions, instant deploy, collaborative build, and debugging tools for integration.
  Remove testing roadblocks. Close the gap that exists with incomplete or capacity
  constrained test environments. Eliminate fees for accessing third-party systems.
  Give QAs access to the exact test environment they need without delays. Streamline
  test environment provisioning time and costs.
image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
x-kinRank: "8"
x-alexaRank: "1165851"
tags: Objects
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/apis.md
specificationVersion: "0.14"
apis:
- name: Salesforce Sandbox Get Version Sobjects
  x-api-slug: salesforce-sandbox
  description: Lists the available objects and their metadata for your organization's
    data. In addition, it provides the organization encoding, as well as maximum batch
    size permitted in queries. For more information, see Internationalization and
    Character Sets (http://www.salesforce.com/us/developer/docs/api/Content/implementation_considerations.htm#sforce_api_other_internationalization).
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://getsandbox.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects
  tags: Version,Sobjects
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjects-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjects-get-openapi.md
- name: Salesforce Sandbox Get Version Sobjects Sobject
  x-api-slug: salesforce-sandbox
  description: Retrieves the metadata for an object.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://getsandbox.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects/{sobject}
  tags: Version,Sobjects,Sobject
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjectssobject-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjectssobject-get-openapi.md
- name: Salesforce Sandbox Post Version Sobjects Sobject
  x-api-slug: salesforce-sandbox
  description: Creates a new object.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://getsandbox.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects/{sobject}
  tags: Version,Sobjects,Sobject
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjectssobject-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjectssobject-post-openapi.md
- name: Salesforce Sandbox Get Version Sobjects Sobject Describe
  x-api-slug: salesforce-sandbox
  description: Completely describes the individual metadata at all levels for the
    specified object. For example, this can be used to retrieve the fields, URLs,
    and child relationships for the Account object.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://getsandbox.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects/{sobject}/describe
  tags: Version,Sobjects,Sobject,Describe
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjectssobjectdescribe-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjectssobjectdescribe-get-openapi.md
- name: Salesforce Sandbox Get Version Sobjects Sobject
  x-api-slug: salesforce-sandbox
  description: Retrieves individual records for an object.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://getsandbox.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects/{sobject}/{id}
  tags: Version,Sobjects,Sobject
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjectssobjectid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjectssobjectid-get-openapi.md
- name: Salesforce Sandbox Delete Version Sobjects Sobject
  x-api-slug: salesforce-sandbox
  description: Deletes a record.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://getsandbox.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects/{sobject}/{id}
  tags: Version,Sobjects,Sobject
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjectssobjectid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjectssobjectid-delete-openapi.md
- name: Salesforce Sandbox Get Version Sobjects Sobject Blobfield
  x-api-slug: salesforce-sandbox
  description: Retrieves the specified blob field from an individual record. Because
    blob fields contain binary data, you can't use JSON or XML to retrieve this data.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://getsandbox.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects/{sobject}/{id}/{blobField}
  tags: Version,Sobjects,Sobject,Blobfield
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjectssobjectidblobfield-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjectssobjectidblobfield-get-openapi.md
- name: Salesforce Sandbox Get Version Sobjects User Password
  x-api-slug: salesforce-sandbox
  description: Gets password expiration status for a given user. The session must
    have permission to access the given user password information, otherwise an error
    response is returned.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://getsandbox.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects/User/{id}/password
  tags: Version,Sobjects,User,Password
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjectsuseridpassword-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjectsuseridpassword-get-openapi.md
- name: Salesforce Sandbox Post Version Sobjects User Password
  x-api-slug: salesforce-sandbox
  description: Changes the password for a given user ID. The new password must conform
    to the password policies for the organization, otherwise you will get an error
    response. You can only change one password per request.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://getsandbox.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects/User/{id}/password
  tags: Version,Sobjects,User,Password
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjectsuseridpassword-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjectsuseridpassword-post-openapi.md
- name: Salesforce Sandbox Delete Version Sobjects User Password
  x-api-slug: salesforce-sandbox
  description: Resets an user password. Salesforce will reset the user password to
    an auto-generated password, which will be returned in the response.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://getsandbox.com
  baseURL: https://na14.salesforce.com//services/data///{version}/sobjects/User/{id}/password
  tags: Version,Sobjects,User,Password
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjectsuseridpassword-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/versionsobjectsuseridpassword-delete-openapi.md
- name: Salesforce Sandbox
  x-api-slug: salesforce-sandbox
  description: Quick and easy mock RESTful API and SOAP webservices. Generate from
    API definitions, instant deploy, collaborative build, and debugging tools for
    integration. Remove testing roadblocks. Close the gap that exists with incomplete
    or capacity constrained test environments. Eliminate fees for accessing third-party
    systems. Give QAs access to the exact test environment they need without delays.
    Streamline test environment provisioning time and costs.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://getsandbox.com
  baseURL: https://na14.salesforce.com//services/data/
  tags: Objects
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce-sandbox/openapi.md
x-common:
- type: x-blog
  url: http://blog.getsandbox.com/
- type: x-twitter
  url: https://twitter.com/_getsandbox
- type: x-website
  url: http://getsandbox.com
- type: x-website
  url: https://getsandbox.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---