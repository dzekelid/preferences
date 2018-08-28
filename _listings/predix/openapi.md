swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
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