---
swagger: "2.0"
x-collection-name: Nordea
x-complete: 0
info:
  title: Nordea Get all payments
  description: Get a list of all payments created for the user
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---