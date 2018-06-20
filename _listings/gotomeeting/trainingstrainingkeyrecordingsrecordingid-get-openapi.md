---
swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 0
info:
  title: Go To Training Get Download for Online Recordings
  description: This call provides the download for the given recording by returning
    a 302 redirect to the original file.
  termsOfService: https://developer.citrixonline.com/terms-use
  contact:
    name: Developer Support
    url: https://developer.citrixonline.com
    email: developer-support@citrixonline.com
  version: 1.0.0
host: api.citrixonline.com
basePath: /G2T/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /trainings/{trainingKey}/recordings:
    get:
      summary: Get Online Recordings for Training
      description: This call retrieves information on all online recordings for a
        given training. If there are none, it returns an empty list.
      operationId: getRecordingsForTraining
      x-api-path-slug: trainingstrainingkeyrecordings-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Trainings
      - TrainingKey
      - Recordings
  /trainings/{trainingKey}/recordings/{recordingId}:
    get:
      summary: Get Download for Online Recordings
      description: This call provides the download for the given recording by returning
        a 302 redirect to the original file.
      operationId: getRecordingDownloadById
      x-api-path-slug: trainingstrainingkeyrecordingsrecordingid-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: recordingId
        description: the unique id of the recording
      responses:
        200:
          description: OK
      tags:
      - Trainings
      - TrainingKey
      - Recordings
      - RecordingId
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