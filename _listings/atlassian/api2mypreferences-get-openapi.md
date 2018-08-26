---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get preference
  description: Returns preference of the currently logged in user. Preference key
    must be provided as input parameter (key). The value is returned exactly as it
    is.
  termsOfService: http://atlassian.com/terms/
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