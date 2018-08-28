swagger: "2.0"
x-collection-name: CallFire
x-complete: 1
info:
  title: CallFire
  description: callfire
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
  /calls/{id}/recordings:
    get:
      summary: Get call recordings for a call
      description: Returns a list of recordings metadata of particular call. Metadata
        contains link to a MP3 recording
      operationId: getCallRecordings
      x-api-path-slug: callsidrecordings-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a call
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Recordings
  /calls/{id}/recordings/{name}:
    get:
      summary: Get call recording by name
      description: Returns recording metadata of particular call. Metadata contains
        link to a MP3 recording
      operationId: getCallRecordingByName
      x-api-path-slug: callsidrecordingsname-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a call
      - in: path
        name: name
        description: A name of a recording
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Recordings
      - Name
  /calls/{id}/recordings/{name}.mp3:
    get:
      summary: Get call mp3 recording by name
      description: Returns a MP3 recording of a particular call, response contains
        binary data, content type is 'audio/mpeg'
      operationId: getCallRecordingMp3ByName
      x-api-path-slug: callsidrecordingsname-mp3-get
      parameters:
      - in: path
        name: id
        description: An id of a call
      - in: path
        name: name
        description: A name of a recording
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Recordings
      - Name.mp3
  /calls/recordings/{id}.mp3:
    get:
      summary: Get call recording in mp3 format
      description: Returns an MP3 recording of particular call, response contains
        binary data, content type is 'audio/mpeg'
      operationId: getCallRecordingMp3
      x-api-path-slug: callsrecordingsid-mp3-get
      parameters:
      - in: path
        name: id
        description: An id of a call
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Recordings.mp3