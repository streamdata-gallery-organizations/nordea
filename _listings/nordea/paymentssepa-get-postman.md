{
  "info": {
    "name": "Nordea Get all payments",
    "_postman_id": "d4746a20-0e29-4258-944f-988e2a60f59a",
    "description": "Get a list of all payments created for the user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "payments",
      "item": [
        {
          "id": "e89e99db-c0d1-43f8-b5bb-8a67cb01cfa7",
          "name": "getPayments",
          "request": {
            "url": "http://api.nordeaopenbanking.com/v2/payments/sepa",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of all payments created for the user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "074506d6-2b37-418b-8b27-4ed79c0d080b"
            }
          ]
        }
      ]
    }
  ]
}