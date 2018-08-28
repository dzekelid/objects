{
  "info": {
    "name": "Microsoft Graph API List Created Objects",
    "_postman_id": "572dfc0e-d2a1-4984-9560-01ab544bf668",
    "description": "List createdObjects Get a list of directory objects that were created by the user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "40e7330a-6afb-4cf9-aecd-7bbf9e4f0869",
          "name": "ListCreatedObjects",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/createdObjects"
              ],
              "variable": [
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "application/json",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List createdObjects Get a list of directory objects that were created by the user"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "d1930252-5327-4d7d-949b-a048f05a84eb"
            }
          ]
        }
      ]
    }
  ]
}