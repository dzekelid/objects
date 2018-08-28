{
  "info": {
    "name": "Microsoft Graph API List Owned Objects",
    "_postman_id": "4109767e-dd3f-4301-87ab-2f5b3d476627",
    "description": "List ownedObjects Get the list of directory objects that are owned by the user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "e0be5232-2bb8-4215-b451-1e6d0bc8f0d7",
          "name": "ListOwnedObjects",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/ownedObjects"
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
                "key": "Accept",
                "value": "{}",
                "description": "application/json",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List ownedObjects Get the list of directory objects that are owned by the user"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "e406ddc9-66c5-41cd-91c6-eda9864e7160"
            }
          ]
        }
      ]
    }
  ]
}