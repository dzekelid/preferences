---
swagger: "2.0"
x-collection-name: CollabNet
x-complete: 0
info:
  title: CollabNet TeamForge API Documentation Gets preference by username
  version: 1.0.0
  description: Gets preference by username.
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{userid}/preferences:
    patch:
      summary: Sets preferences by user id
      description: Sets preferences by user id.
      operationId: setPreferencesById
      x-api-path-slug: usersuseridpreferences-patch
      parameters:
      - in: body
        name: body
        description: Preferences
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Preferences
      - By
      - User
    get:
      summary: Gets preferences by user id
      description: Gets preferences by user id.
      operationId: getPreferencesById
      x-api-path-slug: usersuseridpreferences-get
      parameters:
      - in: path
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Preferences
      - By
      - User
  /users/by-username/{username}/preferences:
    patch:
      summary: Sets preferences by user name
      description: Sets preferences by user name.
      operationId: setPreferences
      x-api-path-slug: usersbyusernameusernamepreferences-patch
      parameters:
      - in: body
        name: body
        description: Preferences
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Preferences
      - By
      - User
      - Name
    get:
      summary: Gets preferences by username
      description: Gets preferences by username.
      operationId: getPreferences
      x-api-path-slug: usersbyusernameusernamepreferences-get
      parameters:
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Preferences
      - By
      - Username
  /users/{userid}/preferences/{preference}:
    get:
      summary: Gets preference by user id
      description: Gets preference by user id.
      operationId: getPreferenceById
      x-api-path-slug: usersuseridpreferencespreference-get
      parameters:
      - in: path
        name: preference
        description: Preference
      - in: path
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Preference
      - By
      - User
  /users/by-username/{username}/preferences/{preference}:
    get:
      summary: Gets preference by username
      description: Gets preference by username.
      operationId: getPreference
      x-api-path-slug: usersbyusernameusernamepreferencespreference-get
      parameters:
      - in: path
        name: preference
        description: Preference
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Preference
      - By
      - Username
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