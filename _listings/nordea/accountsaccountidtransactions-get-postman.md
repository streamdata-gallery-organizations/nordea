{
  "info": {
    "name": "Nordea Get account transactions",
    "_postman_id": "604694c2-26c0-46c3-9c5f-190ff25fd045",
    "description": "Get accounts account transactions",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "accounts",
      "item": [
        {
          "id": "9c30070f-49dc-460d-be49-0f45897708ce",
          "name": "transactionsList",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nordeaopenbanking.com",
              "path": [
                "v2",
                "accounts/:accountId/transactions"
              ],
              "query": [
                {
                  "key": "continuationKey",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "fromDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "language",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "toDate",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get accounts account transactions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a5e54e8-2a07-4212-a57c-e5fe27d92cc4"
            }
          ]
        }
      ]
    }
  ]
}