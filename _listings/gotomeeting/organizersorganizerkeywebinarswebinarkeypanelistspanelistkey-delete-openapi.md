---
swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 0
info:
  title: Go To Webinar Delete webinar panelist
  description: Removes a webinar panelist.
  termsOfService: https://developer.citrixonline.com/terms-use
  contact:
    name: Developer Support
    url: https://developer.citrixonline.com
    email: developer-support@citrixonline.com
  version: 1.0.0
host: api.citrixonline.com
basePath: /G2W/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizers/{organizerKey}/webinars/{webinarKey}/panelists:
    get:
      summary: Get webinar panelists
      description: Retrieves all the panelists for a specific webinar.
      operationId: getPanelists
      x-api-path-slug: organizersorganizerkeywebinarswebinarkeypanelists-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Webinars
      - WebinarKey
      - Panelists
    post:
      summary: Create Panelists
      description: Create panelists for a specified webinar
      operationId: createPanelists
      x-api-path-slug: organizersorganizerkeywebinarswebinarkeypanelists-post
      parameters:
      - in: body
        name: body
        description: Array of panelists
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Webinars
      - WebinarKey
      - Panelists
  /organizers/{organizerKey}/webinars/{webinarKey}/panelists/{panelistKey}:
    delete:
      summary: Delete webinar panelist
      description: Removes a webinar panelist.
      operationId: deleteWebinarPanelist
      x-api-path-slug: organizersorganizerkeywebinarswebinarkeypanelistspanelistkey-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Webinars
      - WebinarKey
      - Panelists
      - PanelistKey
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