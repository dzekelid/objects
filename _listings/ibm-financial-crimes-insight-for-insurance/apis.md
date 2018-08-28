---
name: IBM Financial Crimes Insight for Insurance
x-slug: ibm-financial-crimes-insight-for-insurance
description: IBM&reg; Financial Crimes Insight&reg; for Insurance V3.0, formerly known
  as IBM Counter Fraud Management for Insurance, is now being offered as a cloud service
  offering. It helps organizations analyze data to determine the fraud risk of claims,
  medical providers, and other business entities, manage the full investigation lifecycle,
  and report on outcomes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
x-kinRank: "7"
x-alexaRank: ""
tags: Objects
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/ibm-financial-crimes-insight-for-insurance/apis.md
specificationVersion: "0.14"
apis:
- name: Financial Crimes Insight for Insurance public REST APIs - Get a list of resolved
    objects from resolved entities for a given object.
  x-api-slug: ibmfciplatformfactentitymatch-get
  description: Get a list of resolved objects from resolved entities for a given object.
    Using the provided object ID, produce a list of all objects of the same business
    object type that have been determined to be 'matches'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactentitymatch-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve business
    objects using the specified parameters
  x-api-slug: ibmfciplatformlogical-objectsearch-post
  description: "This method provides searches for business objects within the database.
    \ The results for searching on a time stamp field are affected by the way that
    DB2\xC2\xAE handles time stamps. The JSON string uses ISO format for time stamps,
    such as 2016-06-15T20:11:19.326-04:00. DB2 converts this value to 2016-06-15-20.11.19.326000.
    Because DB2 might add more precision by storing a time stamp as 2016-06-15-20.11.19.326nnnn,
    the search results might not return what is expected. Refer to your DB2 documentation
    for more information on time stamps."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformlogical-objectsearch-post-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Return the existing
    assessments for the object specified
  x-api-slug: ibmfciplatformfacttyperemotesystemremotekeyassessments-get
  description: This service is used to return the existing assessments for the object
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfacttyperemotesystemremotekeyassessments-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Determine if one
    object is a match to the other.
  x-api-slug: ibmfciplatformfactmatch-get
  description: Using the provided objects, determine if one is a 'match' of the other
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactmatch-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Get a list of resolved
    objects from resolved entities for a given object.
  x-api-slug: ibmfciplatformfactentitymatch-get
  description: Get a list of resolved objects from resolved entities for a given object.
    Using the provided object ID, produce a list of all objects of the same business
    object type that have been determined to be 'matches'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactentitymatch-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Insert physical
    object data into the database
  x-api-slug: ibmfciplatformfactphysical-object-put
  description: This method is used to insert physical object data into the database.  The
    XML schema is defined in the PhysicalObject.XSD file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactphysical-object-put-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve a specific
    physical object data from the database, based on its internal id
  x-api-slug: ibmfciplatformfactphysical-objectid-get
  description: This method is used to retrieve specific physical object data from
    the database, based on its internal id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactphysical-objectid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactphysical-objectid-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve a specific
    physical object data from the database, based on its internal id
  x-api-slug: ibmfciplatformfactphysical-objectid-get
  description: This method is used to retrieve specific physical object data from
    the database, based on its internal id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactphysical-objectid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactphysical-objectid-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Insert physical
    object data into the database
  x-api-slug: ibmfciplatformfactphysical-object-put
  description: This method is used to insert physical object data into the database.  The
    XML schema is defined in the PhysicalObject.XSD file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactphysical-object-put-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Get a list of resolved
    objects from resolved entities for a given object.
  x-api-slug: ibmfciplatformfactentitymatch-get
  description: Get a list of resolved objects from resolved entities for a given object.
    Using the provided object ID, produce a list of all objects of the same business
    object type that have been determined to be 'matches'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactentitymatch-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Determine if one
    object is a match to the other.
  x-api-slug: ibmfciplatformfactmatch-get
  description: Using the provided objects, determine if one is a 'match' of the other
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactmatch-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Return the existing
    assessments for the object specified
  x-api-slug: ibmfciplatformfacttyperemotesystemremotekeyassessments-get
  description: This service is used to return the existing assessments for the object
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/objects/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfacttyperemotesystemremotekeyassessments-get-openapi.md
x-common:
- type: x-openapi
  url: https://www.ibm.com/support/knowledgecenter/SSC2HF_3.0.0/api/fcii-insurance-v3.0.0.yaml?origin=swagger-ui
- type: x-pricing
  url: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN#echargex
- type: x-website
  url: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
- type: x-api-gallery
  url: http://ibm.cloud.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ibm.financial.crimes.insight.for.insurance.stack.network
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---