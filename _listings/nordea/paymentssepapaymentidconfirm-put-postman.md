{
  "info": {
    "name": "Nordea Confirm payment",
    "_postman_id": "13c09afc-e2fb-427b-a620-b4e2e79e887a",
    "description": "Start the payment confirmation flow for a payment by payment id",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "payments",
      "item": [
        {
          "id": "89d781ff-47cf-41dd-94cb-5ac852faee32",
          "name": "paymentConfirm",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nordeaopenbanking.com",
              "path": [
                "v2",
                "payments/sepa/:paymentId/confirm"
              ],
              "variable": [
                {
                  "id": "paymentId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
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
            "description": "Start the payment confirmation flow for a payment by payment id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36dc5e82-e6f5-4095-92c4-01a15856e200"
            }
          ]
        }
      ]
    }
  ]
}