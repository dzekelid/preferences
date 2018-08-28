swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/mypreferences:
    get:
      summary: Get preference
      description: Returns preference of the currently logged in user. Preference
        key must be provided as input parameter (key). The value is returned exactly
        as it is.
      operationId: com.atlassian.jira.rest.v2.preference.CurrentUserPreferencesResource.getPreference_get
      x-api-path-slug: api2mypreferences-get
      parameters:
      - in: query
        name: key
        description: \- key of the preference to be returned
      responses:
        200:
          description: OK
      tags:
      - Preference
    put:
      summary: Set preference
      description: Sets preference of the currently logged in user. Preference key
        must be provided as input parameters (key). Value must be provided as POST
        body.
      operationId: com.atlassian.jira.rest.v2.preference.CurrentUserPreferencesResource.setPreference_put
      x-api-path-slug: api2mypreferences-put
      parameters:
      - in: query
        name: key
        description: \- key of the preference to be set
      responses:
        200:
          description: OK
      tags:
      - Set
      - Preference
    delete:
      summary: Remove preference
      description: Removes preference of the currently logged in user. Preference
        key must be provided as input parameters (key).
      operationId: com.atlassian.jira.rest.v2.preference.CurrentUserPreferencesResource.removePreference_delete
      x-api-path-slug: api2mypreferences-delete
      parameters:
      - in: query
        name: key
        description: \- key of the preference to be removed
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Preference