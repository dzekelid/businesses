---
swagger: "2.0"
info:
  title: OpenCorporates Officers  ID
  description: nThis returns information on a particular officer (a director or an
    agent for a company)
  termsOfService: https://opencorporates.com/info/licence
  version: v.04
host: api.opencorporates.com
basePath: v0.4/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /officers/:id:
    get:
      summary: Officers  ID
      description: nThis returns information on a particular officer (a director or
        an agent for a company)
      operationId: officers--id
      parameters:
      - in: query
        name: address
        description: NEWthe given address of the officer, if known (only for users
          with API key)
      - in: query
        name: date_of_birth
        description: NEWthe date of birth of the officer, if known (only for users
          with API key)
      - in: query
        name: end_date
        description: this is date on which the officership ended
      - in: query
        name: position
        description: the position held (e
      - in: query
        name: start_date
        description: this is date on which the officership started
      - in: query
        name: uid
        description: the id given to the officer by the company registry
      responses:
        200:
          description: OK
      tags:
      - businesses
      - officers
definitions: []
x-collection-name: OpenCorporates
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