---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 0
info:
  title: Google Doubleclick API Get Preferred Deal
  version: 1.0.0
  description: Get information about the selected Ad Exchange Preferred Deal.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}/preferreddeals:
    get:
      summary: Get Preferred Deals
      description: List the preferred deals for this Ad Exchange account.
      operationId: adexchangeseller.accounts.preferreddeals.list
      x-api-path-slug: accountsaccountidpreferreddeals-get
      parameters:
      - in: path
        name: accountId
        description: Account owning the deals
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
  /accounts/{accountId}/preferreddeals/{dealId}:
    get:
      summary: Get Preferred Deal
      description: Get information about the selected Ad Exchange Preferred Deal.
      operationId: adexchangeseller.accounts.preferreddeals.get
      x-api-path-slug: accountsaccountidpreferreddealsdealid-get
      parameters:
      - in: path
        name: accountId
        description: Account owning the deal
      - in: path
        name: dealId
        description: Preferred deal to get information about
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
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