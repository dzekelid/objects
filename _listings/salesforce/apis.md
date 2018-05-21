---
name: Salesforce
x-slug: salesforce
description: Salesforce.com Inc. is a global enterprise software company headquartered
  in San Francisco, California. Though best known for its customer relationship management
  (CRM) product, Salesforce has also expanded into the social enterprise arena through
  acquisitions. It is currently ranked the most innovative company in America by Forbes
  magazine, as well as number 27 in Fortunes magazines 100 Best Companies to Work
  For in 2012. As of April 2013, the company is ranked sixth in providing services
  in marketing and customer service automation
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/salesforce-logo.png
x-kinRank: "10"
x-alexaRank: ""
tags: Objects
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce/apis.md
specificationVersion: "0.14"
apis:
- name: SalesForce Get Version Sobjects
  x-api-slug: salesforce
  description: Lists the available objects and their metadata for your organization's
    data. In addition, it provides the organization encoding, as well as maximum batch
    size permitted in queries. For more information, see Internationalization and
    Character Sets (http://www.salesforce.com/us/developer/docs/api/Content/implementation_considerations.htm#sforce_api_other_internationalization).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/salesforce-logo.png
  humanURL: https://developer.salesforce.com/
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects
  tags: Version, Sobjects
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce/versionsobjects-get-openapi.md
- name: SalesForce Get Version Sobjects Sobject
  x-api-slug: salesforce
  description: Retrieves the metadata for an object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/salesforce-logo.png
  humanURL: https://developer.salesforce.com/
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects/{sobject}
  tags: Version, Sobjects, Sobject
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce/versionsobjectssobject-get-openapi.md
- name: SalesForce Add Version Sobjects Sobject
  x-api-slug: salesforce
  description: Creates a new object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/salesforce-logo.png
  humanURL: https://developer.salesforce.com/
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects/{sobject}
  tags: Version, Sobjects, Sobject
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce/versionsobjectssobject-post-openapi.md
- name: SalesForce Get Version Sobjects Sobject Describe
  x-api-slug: salesforce
  description: Completely describes the individual metadata at all levels for the
    specified object. For example, this can be used to retrieve the fields, URLs,
    and child relationships for the Account object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/salesforce-logo.png
  humanURL: https://developer.salesforce.com/
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects/{sobject}/describe
  tags: Version, Sobjects, Sobject, Describe
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce/versionsobjectssobjectdescribe-get-openapi.md
- name: SalesForce Get Version Sobjects Sobject
  x-api-slug: salesforce
  description: Retrieves individual records for an object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/salesforce-logo.png
  humanURL: https://developer.salesforce.com/
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects/{sobject}/{id}
  tags: Version, Sobjects, Sobject
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce/versionsobjectssobjectid-get-openapi.md
- name: SalesForce Delete Version Sobjects Sobject
  x-api-slug: salesforce
  description: Deletes a record.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/salesforce-logo.png
  humanURL: https://developer.salesforce.com/
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects/{sobject}/{id}
  tags: Version, Sobjects, Sobject
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce/versionsobjectssobjectid-delete-openapi.md
- name: SalesForce Get Version Sobjects Sobject  Blobfield
  x-api-slug: salesforce
  description: Retrieves the specified blob field from an individual record. Because
    blob fields contain binary data, you can't use JSON or XML to retrieve this data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/salesforce-logo.png
  humanURL: https://developer.salesforce.com/
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects/{sobject}/{id}/{blobField}
  tags: Version, Sobjects, Sobject, , Blobfield
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce/versionsobjectssobjectidblobfield-get-openapi.md
- name: SalesForce Get Version Sobjects User  Password
  x-api-slug: salesforce
  description: Gets password expiration status for a given user. The session must
    have permission to access the given user password information, otherwise an error
    response is returned.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/salesforce-logo.png
  humanURL: https://developer.salesforce.com/
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects/User/{id}/password
  tags: Version, Sobjects, User, , Password
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce/versionsobjectsuseridpassword-get-openapi.md
- name: SalesForce Add Version Sobjects User  Password
  x-api-slug: salesforce
  description: Changes the password for a given user ID. The new password must conform
    to the password policies for the organization, otherwise you will get an error
    response. You can only change one password per request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/salesforce-logo.png
  humanURL: https://developer.salesforce.com/
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects/User/{id}/password
  tags: Version, Sobjects, User, , Password
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce/versionsobjectsuseridpassword-post-openapi.md
- name: SalesForce Delete Version Sobjects User  Password
  x-api-slug: salesforce
  description: Resets an user password. Salesforce will reset the user password to
    an auto-generated password, which will be returned in the response.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/salesforce-logo.png
  humanURL: https://developer.salesforce.com/
  baseURL: https://na14.salesforce.com//services/data//{version}/sobjects/User/{id}/password
  tags: Version, Sobjects, User, , Password
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce/versionsobjectsuseridpassword-delete-openapi.md
- name: SalesForce
  x-api-slug: salesforce
  description: Salesforce.com Inc. is a global enterprise software company headquartered
    in San Francisco, California. Though best known for its customer relationship
    management (CRM) product, Salesforce has also expanded into the social enterprise
    arena through acquisitions. It is currently ranked the most innovative company
    in America by Forbes magazine, as well as number 27 in Fortunes magazines 100
    Best Companies to Work For in 2012. As of April 2013, the company is ranked sixth
    in providing services in marketing and customer service automation
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/salesforce-logo.png
  humanURL: https://developer.salesforce.com/
  baseURL: https://na14.salesforce.com//services/data
  tags: Objects
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/salesforce/openapi.md
x-common:
- type: x-base
  url: https://na1.salesforce.com
- type: x-blog
  url: https://developer.salesforce.com/blogs/
- type: x-blog-rss
  url: http://feeds.feedburner.com/SforceBlog
- type: x-crunchbase
  url: http://www.crunchbase.com/company/salesforce
- type: x-github
  url: https://github.com/salesforce
- type: x-partners
  url: https://partners.salesforce.com/
- type: x-twitter
  url: https://twitter.com/salesforcedevs
- type: x-website
  url: https://developer.salesforce.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---