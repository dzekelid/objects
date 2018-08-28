{
  "info": {
    "name": "My Space Get Activities Supported Object Types",
    "_postman_id": "2f0a10f9-1dea-449a-98ef-ceab3546513c",
    "description": "Retrieves all supported object types.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Activities",
      "item": [
        {
          "id": "17c1e801-b6d4-49ba-8de0-61b4ced54df9",
          "name": "1.0.activities.personId.selector.appId.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.myspace.com",
              "path": [
                "1.0/activities/:personId/:selector/:appId"
              ],
              "query": [
                {
                  "key": "count",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startIndex",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "updatedSince",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "appId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "personId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "selector",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves activities created by an application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c5f6f1b-81ae-459d-86bd-0339e1466d6b"
            }
          ]
        },
        {
          "id": "3b9eafb6-c802-4064-b197-a45e90070705",
          "name": "1.0.activities._supportedObjectTypes.get",
          "request": {
            "url": "http://api.myspace.com/1.0/activities/@supportedObjectTypes?count=%7B%7D&fields=%7B%7D&format=%7B%7D&startIndex=%7B%7D&updatedSince=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves all supported object types."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd0d1201-48da-4624-8267-4128e152c1bc"
            }
          ]
        }
      ]
    }
  ]
}