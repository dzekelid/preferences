swagger: "2.0"
x-collection-name: CollabNet
x-complete: 1
info:
  title: Foundation API
  version: 1.0.0
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
  /users/myself/preferences:
    patch:
      summary: Sets preferences for current user
      description: Sets preferences for current user.
      operationId: setPreferencesForMyself
      x-api-path-slug: usersmyselfpreferences-patch
      parameters:
      - in: body
        name: body
        description: Preferences
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Preferencescurrent
      - User
    get:
      summary: Gets preferences for current user
      description: Gets preferences for current user.
      operationId: getPreferencesForMyself
      x-api-path-slug: usersmyselfpreferences-get
      responses:
        200:
          description: OK
      tags:
      - Preferencescurrent
      - User