---
name: GoToMeeting
x-slug: gotomeeting
description: Citrix enables business mobility through the secure delivery of apps
  and data to any device on any network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
x-kinRank: "7"
x-alexaRank: "7422"
tags: Recordings
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/recordings/master/_listings/gotomeeting/apis.md
specificationVersion: "0.14"
apis:
- name: Go To Training Get Online Recordings for Training
  x-api-slug: go-to-training
  description: This call retrieves information on all online recordings for a given
    training. If there are none, it returns an empty list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest//trainings/{trainingKey}/recordings
  tags: Trainings,TrainingKey,Recordings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recordings/master/_listings/gotomeeting/trainingstrainingkeyrecordings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recordings/master/_listings/gotomeeting/trainingstrainingkeyrecordings-get-openapi.md
- name: Go To Training Get Download for Online Recordings
  x-api-slug: go-to-training
  description: This call provides the download for the given recording by returning
    a 302 redirect to the original file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest//trainings/{trainingKey}/recordings/{recordingId}
  tags: Trainings,TrainingKey,Recordings,RecordingId
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recordings/master/_listings/gotomeeting/trainingstrainingkeyrecordingsrecordingid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recordings/master/_listings/gotomeeting/trainingstrainingkeyrecordingsrecordingid-get-openapi.md
- name: Go To Training
  x-api-slug: go-to-training
  description: Citrix enables business mobility through the secure delivery of apps
    and data to any device on any network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Recordings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recordings/master/_listings/gotomeeting/openapi.md
x-common:
- type: x-base
  url: https://api.citrixonline.com
- type: x-blog
  url: http://blogs.citrix.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/citrix-systems
- type: x-crunchbase
  url: http://www.crunchbase.com/company/citrix-systems
- type: x-developer
  url: https://developer.citrixonline.com/
- type: x-email
  url: secure@citrix.com
- type: x-email
  url: americasconsulting@citrix.com
- type: x-email
  url: poland@citrix.com
- type: x-email
  url: citrix_ru@citrix.com
- type: x-email
  url: Licensing-emea@eu.citrix.com
- type: x-email
  url: eduardo.fleites@citrix.com
- type: x-email
  url: CitrixReady@citrix.com
- type: x-email
  url: CSP@citrix.com
- type: x-email
  url: partneroperationsEMEA@eu.citrix.com
- type: x-github
  url: https://github.com/citrix
- type: x-twitter
  url: https://twitter.com/gotomeeting
- type: x-twitter
  url: https://twitter.com/citrix
- type: x-website
  url: https://citrixonline.com
- type: x-website
  url: http://citrixonline.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---