---
swagger: "2.0"
x-collection-name: Nordea
x-complete: 1
info:
  title: Nordea
  description: the-nordeas-open-banking-initiative-obi-api-offers-a-safe-and-simple-way-to-try-out-the-upcoming-obi-this-api-is-a-sandbox-version-and-its-purpose-is-to-make-developers-familiar-with-the-upcoming-obi-production-release-moreover-it-allows-the-developers-to-experiment-and-build-applications-which-use-the-obi-before-its-official-release-
  contact:
    name: Open Banking team
  version: 1.0.0
host: api.nordeaopenbanking.com
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts:
    get:
      summary: List accounts
      description: Get accounts
      operationId: accountList
      x-api-path-slug: accounts-get
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /accounts/{accountId}:
    get:
      summary: Get account details by account id
      description: Get accounts account
      operationId: accountDetails
      x-api-path-slug: accountsaccountid-get
      parameters:
      - in: path
        name: accountId
        description: Internal account identifier
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Account
  /accounts/{accountId}/transactions:
    get:
      summary: Get account transactions
      description: Get accounts account transactions
      operationId: transactionsList
      x-api-path-slug: accountsaccountidtransactions-get
      parameters:
      - in: path
        name: accountId
        description: Internal account identifier
      - in: query
        name: continuationKey
        description: Resource listing may return a continuationKey if theres more
          results available
      - in: query
        name: fromDate
        description: List transactions starting from and including this date
      - in: query
        name: language
        description: Preferred language for textual values
      - in: query
        name: toDate
        description: List transactions until and including this date
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Account
      - Transactions
  /payments/sepa:
    get:
      summary: Get all payments
      description: Get a list of all payments created for the user
      operationId: getPayments
      x-api-path-slug: paymentssepa-get
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Sepa
    post:
      summary: Initiate payment
      description: Post payments
      operationId: paymentInitiate
      x-api-path-slug: paymentssepa-post
      parameters:
      - in: body
        name: createPaymentRequestV2
        description: Request to create a new payment
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Response-Scenarios
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Sepa
  /payments/sepa/{paymentId}:
    get:
      summary: Get payment
      description: Get v2 payments sepa payment
      operationId: getPayment
      x-api-path-slug: paymentssepapaymentid-get
      parameters:
      - in: path
        name: paymentId
        description: Payment id of the payment to get
      - in: header
        name: X-Response-Scenarios
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Sepa
      - Payment
  /payments/sepa/{paymentId}/confirm:
    put:
      summary: Confirm payment
      description: Start the payment confirmation flow for a payment by payment id
      operationId: paymentConfirm
      x-api-path-slug: paymentssepapaymentidconfirm-put
      parameters:
      - in: path
        name: paymentId
        description: Payment id of the payment to confirm
      - in: header
        name: X-Response-Scenarios
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Sepa
      - Payment
      - Confirm
---