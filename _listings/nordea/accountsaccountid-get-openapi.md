---
swagger: "2.0"
x-collection-name: Nordea
x-complete: 0
info:
  title: Nordea Get account details by account id
  description: Get accounts account
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