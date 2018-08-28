---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix AppHub ARCS Delete the preferences information
  description: Delete the preferences information
  termsOfService: Terms of service
  contact:
    name: 'Digital Predix AppHub ARCS: Development'
  version: 1.0.0
host: predix-apphub-arcs-prod.run.aws-usw02-pr.ice.predix.io
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /preferences:
    get:
      summary: Get the preferences information
      description: Get the preferences information
      operationId: getPreferenceUsingGET
      x-api-path-slug: preferences-get
      responses:
        200:
          description: OK
      tags:
      - Preferences
    post:
      summary: Save the preferences information
      description: save the preferences information
      operationId: savePreferenceUsingPOST
      x-api-path-slug: preferences-post
      parameters:
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Preferences
  /preferences/{uuid}:
    put:
      summary: Update the preferences information
      description: Update the preferences information
      operationId: updatePreferenceUsingPUT
      x-api-path-slug: preferencesuuid-put
      parameters:
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - Preferences
      - Uuid
    delete:
      summary: Delete the preferences information
      description: Delete the preferences information
      operationId: deletePreferenceUsingDELETE
      x-api-path-slug: preferencesuuid-delete
      parameters:
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - Preferences
      - Uuid
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