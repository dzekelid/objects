{
  "info": {
    "name": "Plentymarkets Get assigend metadata for a single storage object",
    "_postman_id": "22289bc9-cf5f-44b2-8e96-77fd95f762c4",
    "description": "Get assigend metadata for a single storage object.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Single",
      "item": [
        {
          "id": "6bbea7fc-033d-4b9a-8336-488b9275fd0c",
          "name": "getRestAccountsContactsContactDocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/contacts/:contactId/document"
              ],
              "query": [
                {
                  "key": "key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "contactId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a single storage object from contact documents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef49725d-ddec-4290-977f-e78dc0400f2d"
            }
          ]
        }
      ]
    },
    {
      "name": "Temporary",
      "item": [
        {
          "id": "070f1e34-ca42-45b3-8b1e-fe4b19aad324",
          "name": "getRestAccountsContactsContactDocumentUrl",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/contacts/:contactId/document/url"
              ],
              "query": [
                {
                  "key": "key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "contactId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a temporary url for a single document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ad9b649-04e6-4403-8861-7faaea79a4a2"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "afc950dc-873c-42a7-bd22-3b42edeed214",
          "name": "getRestAccountsContactsContactDocuments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/contacts/:contactId/documents"
              ],
              "query": [
                {
                  "key": "continuationToken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "contactId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List documents for a single contact."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6759a8b7-9166-489c-a7c7-8e4c221f0627"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "0ef61e82-66bd-45c8-b273-b91a795d5704",
          "name": "getRestBoardsBoard",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/boards/:boardId"
              ],
              "query": [
                {
                  "key": "tasksPerPage",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "boardId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets a single board by its id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bfffc277-10e3-436b-bcae-f419e2ce2dfa"
            }
          ]
        }
      ]
    },
    {
      "name": "Returns",
      "item": [
        {
          "id": "b51ae78b-f504-4fde-a682-12a402c634ea",
          "name": "getRestCustomerContractsContract",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/customer_contracts/:contractId"
              ],
              "variable": [
                {
                  "id": "contractId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a single contract."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9abb0149-3584-4ecd-af5f-016d6e827f02"
            }
          ]
        }
      ]
    },
    {
      "name": "File",
      "item": [
        {
          "id": "e99a4d09-8564-497f-a5c4-8ca55aa1ee92",
          "name": "getRestStorageFrontendFile",
          "request": {
            "url": "http://example.com/rest/storage/frontend/file?key=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get file information for a single object in frontend storage. append public cloudfront url to retrieved object.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e780618-d45c-4ddc-b6dd-2225d952a253"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "0dee5f61-3f94-49d7-919e-bb690905b6fe",
          "name": "postRestStorageFrontendFile",
          "request": {
            "url": "http://example.com/rest/storage/frontend/file?key=%7B%7D&maxAge=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "If file is an image, generate a thumbnail and store dimensions in metadata."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9dd26e8-2051-4734-b87a-e9ecd9470d7b"
            }
          ]
        }
      ]
    },
    {
      "name": "Remove",
      "item": [
        {
          "id": "0615a32d-d36d-45e7-98d7-b59993cabd64",
          "name": "deleteRestStorageFrontendFile",
          "request": {
            "url": "http://example.com/rest/storage/frontend/file?key=%7B%7D",
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Remove a single object from frontend storage.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80d91292-a198-4869-8325-e68a63f32370"
            }
          ]
        }
      ]
    },
    {
      "name": "Assigend",
      "item": [
        {
          "id": "66a24b81-0d26-4d45-baf4-07cf009055db",
          "name": "getRestStorageFrontendFileMetadata",
          "request": {
            "url": "http://example.com/rest/storage/frontend/file/metadata?key=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get assigend metadata for a single storage object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ab34a4a-4eee-4277-9c32-7cd7234f757b"
            }
          ]
        }
      ]
    }
  ]
}