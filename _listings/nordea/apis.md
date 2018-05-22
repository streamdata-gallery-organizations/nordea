---
name: Nordea
x-slug: nordea
description: The Nordeas Open Banking Initiative (OBI) API, offers a safe and simple
  way to try out the upcoming OBI. This API is a sandbox version, and its purpose
  is to make developers familiar with the upcoming OBI production release. Moreover,
  it allows the developers to experiment and build applications which use the OBI
  before its official release.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/nordea-bank-logo.png
x-kinRank: "8"
x-alexaRank: ""
tags: Nordea
created: "2018-05-22"
modified: "2018-05-22"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nordea/master/_listings/nordea/apis.md
specificationVersion: "0.14"
apis:
- name: Nordea List accounts
  x-api-slug: nordea
  description: Get accounts
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/nordea-bank-logo.png
  humanURL: https://nordeaopenbanking.com
  baseURL: https://api.nordeaopenbanking.com/v2///accounts
  tags: Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nordea/master/_listings/nordea/accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nordea/master/_listings/nordea/accounts-get-openapi.md
- name: Nordea Get account details by account id
  x-api-slug: nordea
  description: Get accounts account
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/nordea-bank-logo.png
  humanURL: https://nordeaopenbanking.com
  baseURL: https://api.nordeaopenbanking.com/v2///accounts/{accountId}
  tags: Accounts, Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nordea/master/_listings/nordea/accountsaccountid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nordea/master/_listings/nordea/accountsaccountid-get-openapi.md
- name: Nordea Get account transactions
  x-api-slug: nordea
  description: Get accounts account transactions
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/nordea-bank-logo.png
  humanURL: https://nordeaopenbanking.com
  baseURL: https://api.nordeaopenbanking.com/v2///accounts/{accountId}/transactions
  tags: Accounts, Account, Transactions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nordea/master/_listings/nordea/accountsaccountidtransactions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nordea/master/_listings/nordea/accountsaccountidtransactions-get-openapi.md
- name: Nordea Get all payments
  x-api-slug: nordea
  description: Get a list of all payments created for the user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/nordea-bank-logo.png
  humanURL: https://nordeaopenbanking.com
  baseURL: https://api.nordeaopenbanking.com/v2///payments/sepa
  tags: Payments, Sepa
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nordea/master/_listings/nordea/paymentssepa-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nordea/master/_listings/nordea/paymentssepa-get-openapi.md
- name: Nordea Initiate payment
  x-api-slug: nordea
  description: Post payments
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/nordea-bank-logo.png
  humanURL: https://nordeaopenbanking.com
  baseURL: https://api.nordeaopenbanking.com/v2///payments/sepa
  tags: Payments, Sepa
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nordea/master/_listings/nordea/paymentssepa-post-openapi.md
- name: Nordea Get payment
  x-api-slug: nordea
  description: Get v2 payments sepa payment
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/nordea-bank-logo.png
  humanURL: https://nordeaopenbanking.com
  baseURL: https://api.nordeaopenbanking.com/v2///payments/sepa/{paymentId}
  tags: Payments, Sepa, Payment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nordea/master/_listings/nordea/paymentssepapaymentid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nordea/master/_listings/nordea/paymentssepapaymentid-get-openapi.md
- name: Nordea Confirm payment
  x-api-slug: nordea
  description: Start the payment confirmation flow for a payment by payment id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/nordea-bank-logo.png
  humanURL: https://nordeaopenbanking.com
  baseURL: https://api.nordeaopenbanking.com/v2///payments/sepa/{paymentId}/confirm
  tags: Payments, Sepa, Payment, Confirm
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nordea/master/_listings/nordea/paymentssepapaymentidconfirm-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nordea/master/_listings/nordea/paymentssepapaymentidconfirm-put-openapi.md
- name: Nordea
  x-api-slug: nordea
  description: The Nordeas Open Banking Initiative (OBI) API, offers a safe and simple
    way to try out the upcoming OBI. This API is a sandbox version, and its purpose
    is to make developers familiar with the upcoming OBI production release. Moreover,
    it allows the developers to experiment and build applications which use the OBI
    before its official release.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/nordea-bank-logo.png
  humanURL: https://nordeaopenbanking.com
  baseURL: https://api.nordeaopenbanking.com/v2/
  tags: Nordea
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nordea/master/_listings/nordea/openapi.md
x-common:
- type: x-blog
  url: https://medium.com/@NordeaOpenBanking
- type: x-blog-rss
  url: https://medium.com/feed/@NordeaOpenBanking
- type: x-developer
  url: https://developer.nordeaopenbanking.com/
- type: x-documentation
  url: https://developer.nordeaopenbanking.com/app/docs
- type: x-email
  url: openbankingsupport@nordea.com
- type: x-github
  url: https://github.com/NordeaOSS
- type: x-privacy-policy
  url: https://developer.nordeaopenbanking.com/app/page/privacy
- type: x-terms-of-service
  url: https://developer.nordeaopenbanking.com/app/page/terms
- type: x-twitter
  url: https://twitter.com/NordeaAPI
- type: x-website
  url: https://nordeaopenbanking.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---