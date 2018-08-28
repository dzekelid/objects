---
name: Microsoft Graph
x-slug: microsoft-graph
description: 'Microsoft Graph exposes multiple APIs from Office 365 and other Microsoft
  cloud services through a single endpoint: https://graph.microsoft.com. Microsoft
  Graph simplifies queries that would otherwise be more complex. You can use Microsoft
  Graph to: Access data from multiple Microsoft cloud services, including Azure Active
  Directory, Exchange Online as part of Office 365, SharePoint, OneDrive, OneNote,
  and Planner. Navigate between entities and relationships. Access intelligence and
  insights from the Microsoft cloud (for commercial users).'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Objects
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/apis.md
specificationVersion: "0.14"
apis:
- name: Microsoft Graph API - Get Member Objects
  x-api-slug: megetmemberobjects-post
  description: Get member objects Returns all the groups and directory roles that
    a user, group, or directory object is a member of. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/megetmemberobjects-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/megetmemberobjects-post-openapi.md
- name: Microsoft Graph API - Get Member Objects
  x-api-slug: usersid--userprincipalnamegetmemberobjects-post
  description: Get member objects Returns all the groups and directory roles that
    a user, group, or directory object is a member of. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/usersid--userprincipalnamegetmemberobjects-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/usersid--userprincipalnamegetmemberobjects-post-openapi.md
- name: Microsoft Graph API - Get Member Objects
  x-api-slug: directoryobjectsidgetmemberobjects-post
  description: Get member objects Returns all the groups and directory roles that
    a user, group, or directory object is a member of. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/directoryobjectsidgetmemberobjects-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/directoryobjectsidgetmemberobjects-post-openapi.md
- name: Microsoft Graph API - Group Get Member Objects
  x-api-slug: groupsidgetmemberobjects-post
  description: 'group: getMemberObjects Return all of the groups that this group is
    a member of. The check is transitive. Note: Groups cannot be members of directory
    roles, so no directory roles will be returned.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/groupsidgetmemberobjects-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/groupsidgetmemberobjects-post-openapi.md
- name: Microsoft Graph API - List Created Objects
  x-api-slug: usersid--userprincipalnamecreatedobjects-get
  description: List createdObjects Get a list of directory objects that were created
    by the user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/usersid--userprincipalnamecreatedobjects-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/usersid--userprincipalnamecreatedobjects-get-openapi.md
- name: Microsoft Graph API - List Owned Objects
  x-api-slug: usersid--userprincipalnameownedobjects-get
  description: List ownedObjects Get the list of directory objects that are owned
    by the user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/usersid--userprincipalnameownedobjects-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/usersid--userprincipalnameownedobjects-get-openapi.md
- name: Microsoft Graph API - Delete Directory Object
  x-api-slug: directoryobjectsid-delete
  description: Delete directoryObject Deletes a directoryObject.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/directoryobjectsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/directoryobjectsid-delete-openapi.md
- name: Microsoft Graph API - Get Directory Object
  x-api-slug: directoryobjectsid-get
  description: Get directoryObject Retrieve the properties and relationships of directoryObject
    object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/directoryobjectsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/directoryobjectsid-get-openapi.md
- name: Microsoft Graph API - Get Directory Object
  x-api-slug: directoryobjectsid-get
  description: Get directoryObject Retrieve the properties and relationships of directoryObject
    object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/directoryobjectsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/directoryobjectsid-get-openapi.md
- name: Microsoft Graph API - Delete Directory Object
  x-api-slug: directoryobjectsid-delete
  description: Delete directoryObject Deletes a directoryObject.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/directoryobjectsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/microsoft-graph/directoryobjectsid-delete-openapi.md
x-common:
- type: x-api-gallery
  url: http://messente.api.gallery.streamdata.io
- type: x-api-stack
  url: http://microsoft.graph.stack.network
- type: x-change-loge
  url: https://developer.microsoft.com/en-us/graph/docs/overview/changelog
- type: x-documentation
  url: https://developer.microsoft.com/en-us/graph/docs
- type: x-explorer
  url: https://developer.microsoft.com/en-us/graph/graph-explorer
- type: x-getting-started
  url: https://developer.microsoft.com/en-us/graph/docs/get-started/rest
- type: x-github
  url: https://github.com/microsoftgraph
- type: x-sdk
  url: https://developer.microsoft.com/en-us/graph/code-samples-and-sdks
- type: x-website
  url: https://developer.microsoft.com/en-us/graph/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---