{
  "info": {
    "name": "Nordea List accounts",
    "_postman_id": "afb28fc2-e925-45d1-8a45-26fc3f66c470",
    "description": "Get accounts",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Accounts",
      "item": [
        {
          "id": "11f47f49-a670-467c-8ea2-f5ffb559d47e",
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
              "id": "d45ff378-e888-44b9-ba04-20d17eaf087b"
            }
          ]
        }
      ]
    }
  ]
}