---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Calendar Get Multiple Event Details
  description: Get the details for the specified events.
  version: 1.0.0
host: www.xignite.com
basePath: xCalendar.json/XigniteCalendar
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetEventDetails:
    get:
      summary: Get Event Details
      description: Get the details for the specified event.
      operationId: postGeteventdetails
      x-api-path-slug: geteventdetails-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Event
      - Details
  /GetMultipleEventDetails:
    get:
      summary: Get Multiple Event Details
      description: Get the details for the specified events.
      operationId: postGetmultipleeventdetails
      x-api-path-slug: getmultipleeventdetails-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Multiple
      - Event
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