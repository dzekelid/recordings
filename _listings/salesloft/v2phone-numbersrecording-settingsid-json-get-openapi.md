---
swagger: "2.0"
x-collection-name: SalesLoft
x-complete: 0
info:
  title: SalesLoft Fetch recording setting
  description: |-
    Fetches the recording status for a given phone number, based on Do Not Record and Recording Governance for your team.
    Phone number should be in E.164 format.
  version: v2
host: api.salesloft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/phone_numbers/recording_settings/{id}.json:
    get:
      summary: Fetch recording setting
      description: |-
        Fetches the recording status for a given phone number, based on Do Not Record and Recording Governance for your team.
        Phone number should be in E.164 format.
      operationId: v2.phone_numbers.recording_settings.id.json.get
      x-api-path-slug: v2phone-numbersrecording-settingsid-json-get
      parameters:
      - in: path
        name: id
        description: E
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Recording
      - Setting
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