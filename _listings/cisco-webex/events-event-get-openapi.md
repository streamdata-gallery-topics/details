---
swagger: "2.0"
x-collection-name: Cisco WebEx
x-complete: 0
info:
  title: Webex Teams Admin API Get Events Details
  description: "Shows details for an event, by event ID.\r\nSpecify the event ID in
    the eventId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-events-eventId-get.html"
  version: 1.0.0
host: api.ciscospark.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /licenses/{_license}:
    get:
      summary: Get License Details
      description: "Shows details for a license, by ID.\r\n\r\nSpecify the license
        ID in the licenseId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-licenses-licenseId-get.html\r\n\r\nExample
        Response:\r\n``` json\r\n{\r\n  'id' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',\r\n
        \ 'displayName' : 'Spark Calling',\r\n  'totalUnits' : '42',\r\n  'consumedUnits'
        : \"8'\r\n}\r\n```"
      operationId: LicensesByLicenseGet
      x-api-path-slug: licenses-license-get
      parameters:
      - in: path
        name: _license
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - License
      - Details
  /roles/{_role}:
    get:
      summary: Get Role Details
      description: |-
        Shows details for a role, by ID.

        Specify the role ID in the roleId parameter in the URI.

        https://developer.webex.com/endpoint-roles-roleId-get.html

        Example Response:
        ``` json
        {
          'id' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',
          'displayName' : 'Full Administrator'
        }
        ```
      operationId: RolesByRoleGet
      x-api-path-slug: roles-role-get
      parameters:
      - in: path
        name: _role
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Role
      - Details
  /people/me:
    get:
      summary: Get Person Details (me)
      description: |-
        Show the profile for the authenticated user.

        https://developer.webex.com/endpoint-people-me-get.html
      operationId: PeopleMeGet
      x-api-path-slug: peopleme-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Person
      - Details
      - (me)
  /events/{_event}:
    get:
      summary: Get Events Details
      description: "Shows details for an event, by event ID.\r\nSpecify the event
        ID in the eventId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-events-eventId-get.html"
      operationId: EventsByEventGet
      x-api-path-slug: events-event-get
      parameters:
      - in: path
        name: _event
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Events
      - Details
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