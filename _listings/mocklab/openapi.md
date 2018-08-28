swagger: "2.0"
x-collection-name: MockLab
x-complete: 1
info:
  title: WireMock
  version: 1.0.0
basePath: /__admin
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /recordings/snapshot:
    post:
      summary: Post Recordings Snapshot
      description: Take a snapshot recording
      operationId: postRecordingsSnapshot
      x-api-path-slug: recordingssnapshot-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Recordings
      - Snapshot
  /recordings/start:
    post:
      summary: Post Recordings Start
      description: Start recording stub mappings
      operationId: postRecordingsStart
      x-api-path-slug: recordingsstart-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Recordings
      - Start
  /recordings/status:
    get:
      summary: Get Recordings Status
      description: Get the recording status (started or stopped)
      operationId: getRecordingsStatus
      x-api-path-slug: recordingsstatus-get
      responses:
        200:
          description: Successful response
      tags:
      - Recordings
      - Status
  /recordings/stop:
    post:
      summary: Post Recordings Stop
      description: Stop recording stub mappings
      operationId: postRecordingsStop
      x-api-path-slug: recordingsstop-post
      responses:
        200:
          description: Successful response
      tags:
      - Recordings
      - Stop