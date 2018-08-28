swagger: "2.0"
x-collection-name: SalesLoft
x-complete: 1
info:
  title: SalesLoft
  description: salesloft-helps-transform-sales-teams-into-modern-sales-organizations---converting-more-target-accounts-into-customer-accounts
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