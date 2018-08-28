swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/pref:
    get:
      summary: Retrieve User Preferences
      description: User preferences for non-state information, such as Layout designer
        zoom levels
      operationId: userPrefGet
      x-api-path-slug: userpref-get
      parameters:
      - in: formData
        name: preference
        description: An optional preference
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - User
      - Preferences
    post:
      summary: Save User Preferences
      description: Save User preferences for non-state information, such as Layout
        designer zoom levels
      operationId: userPrefEdit
      x-api-path-slug: userpref-post
      parameters:
      - in: body
        name: preference
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Save
      - User
      - Preferences