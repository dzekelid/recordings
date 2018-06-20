---
swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 1
info:
  title: Go To Training
  description: the-gototraining-api-enables-developers-to-use-the-stable-and-robust-gototraining-functionality-as-the-basis-for-online-trainings-in-a-proprietary-learning-management-system--the-gototraining-apis-provide-the-ability-to-access-the-scheduling-registration-management-and-reporting-functions-of-gototraining-from-external-applications--with-the-ability-to-tightly-integrate-gototraining-into-your-learning-infrastructure-you-can-offer-your-learners-a-seamless-user-experience-and-provide-them-with-a-market-leading-virtual-classroom-environment-
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
---