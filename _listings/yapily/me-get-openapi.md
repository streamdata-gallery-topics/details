---
swagger: "2.0"
x-collection-name: Yapily
x-complete: 0
info:
  title: Yapily Returns the details of the application which owns the request credentials
  description: Returns the details of the application which owns the request credentials.
  version: 1.0.0
host: api.yapily.com:443
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /institutions/{institutionId}:
    get:
      summary: Retrieves details of a specific institution available in Yapily
      description: Retrieves details of a specific institution available in yapily.
      operationId: getInstitutionUsingGET
      x-api-path-slug: institutionsinstitutionid-get
      parameters:
      - in: path
        name: institutionId
        description: institutionId
      responses:
        200:
          description: OK
      tags:
      - Retrieves
      - Details
      - Specific
      - Institution
      - Available
      - In
      - Yapily
  /institutions/{institutionId}/personal-current-accounts:
    get:
      summary: Retrieves details of personal current accounts for an institution
      description: Retrieves details of personal current accounts for an institution.
      operationId: getPersonalCurrentAccountsUsingGET
      x-api-path-slug: institutionsinstitutionidpersonalcurrentaccounts-get
      parameters:
      - in: path
        name: institutionId
        description: institutionId
      responses:
        200:
          description: OK
      tags:
      - Retrieves
      - Details
      - Personal
      - Current
      - Accountsan
      - Institution
  /me:
    get:
      summary: Returns the details of the application which owns the request credentials
      description: Returns the details of the application which owns the request credentials.
      operationId: getApplicationMeUsingGET
      x-api-path-slug: me-get
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Details
      - Application
      - Which
      - Owns
      - Request
      - Credentials
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