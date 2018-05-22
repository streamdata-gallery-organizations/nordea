{
  "info": {
    "name": "Nordea Get account details by account id",
    "_postman_id": "90ff5e18-4ae1-4478-b8e1-9576656b419e",
    "description": "Get accounts account",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Accounts",
      "item": [
        {
          "id": "36e2826e-2b62-4d3c-b121-1d1e25048759",
          "name": "accountList",
          "request": {
            "url": "http://api.nordeaopenbanking.com/v2/accounts",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get accounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94e20991-f110-4539-a096-dbb45d850507"
            }
          ]
        },
        {
          "id": "1b2f5658-d5a8-4ae6-9471-d485379f5155",
          "name": "accountDetails",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nordeaopenbanking.com",
              "path": [
                "v2",
                "accounts/:accountId"
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
            "description": "Get accounts account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02541a06-207c-4285-9de8-dbe5c21d86e5"
            }
          ]
        }
      ]
    }
  ]
}