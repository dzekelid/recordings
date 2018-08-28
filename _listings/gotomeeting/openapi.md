swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 1
info:
  title: SCIM
  description: the-scim-api-lets-you-manage-users-in-your-organization--you-can-then-automate-the-provisioning-of-product-licenses-for-these-users-and-they-can-use-your-companys-single-signon-solution-through-an-identity-provider-
  termsOfService: https://developer.citrixonline.com/terms-use
  contact:
    name: Developer Support
    url: https://developer.citrixonline.com
    email: developer-support@citrixonline.com
  version: N/A
host: api.citrixonline.com
basePath: /identity/v1
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