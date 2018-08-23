---
swagger: "2.0"
info:
  title: OpenCorporates Placeholder  ID
  description: nA placeholder is we call something we believe is probably a company
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
  /placeholder/:id:
    get:
      summary: Placeholder  ID
      description: nA placeholder is we call something we believe is probably a company
      operationId: placeholder--id
      parameters:
      - in: query
        name: company
        description: if the placeholder has been matched to a company, the company
          will be included, together with basic information for the company
      - in: query
        name: identifier
        description: an identifier that is associated with the placeholder, for example
          an SEC CIK code
      - in: query
        name: jurisdiction_code
        description: the code for the jurisdiction in which the placeholder is believed
          to be incorporated (see [GET company](#company))
      - in: query
        name: jurisdiction_string
        description: A plain text representation for the jurisdiction in which the
          placeholder is believed to be incorporated - this may be the name of a jurisdiction,
          of a country, or possibly an ISO 3166-2 code
      - in: query
        name: name
        description: the name of the entity
      - in: query
        name: opencorporates_url
        description: the url of the placeholder
      responses:
        200:
          description: OK
      tags:
      - businesses
      - placeholder
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