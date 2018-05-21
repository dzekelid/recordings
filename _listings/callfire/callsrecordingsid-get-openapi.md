---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 0
info:
  title: Callfire Get call recording by id
  description: Returns metadata of recording of a particular call. Metadata contains
    a link to a MP3 recording
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /calls/recordings/{id}:
    get:
      summary: Get call recording by id
      description: Returns metadata of recording of a particular call. Metadata contains
        a link to a MP3 recording
      operationId: getCallRecording
      x-api-path-slug: callsrecordingsid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: "~"
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Recordings
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