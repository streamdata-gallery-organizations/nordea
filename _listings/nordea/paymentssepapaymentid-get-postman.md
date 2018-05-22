{
  "info": {
    "name": "Nordea Get payment",
    "_postman_id": "6f789bf2-78a8-4a31-9720-3adc44a98b1e",
    "description": "Get v2 payments sepa payment",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "payments",
      "item": [
        {
          "id": "0fb2096f-e2e0-4da4-aab7-22b01372d56a",
          "name": "getPayment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nordeaopenbanking.com",
              "path": [
                "v2",
                "payments/sepa/:paymentId"
              ],
              "variable": [
                {
                  "id": "paymentId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "X-Response-Scenarios",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get v2 payments sepa payment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28926d8d-f5fa-4bab-9698-8172049ab7d7"
            }
          ]
        }
      ]
    }
  ]
}