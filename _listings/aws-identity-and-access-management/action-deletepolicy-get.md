---
swagger: "2.0"
info:
  title: AWS Identity and Access Management API Delete Policy
  version: 1.0.0
  description: Deletes the specified managed policy.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeletePolicy:
    get:
      summary: ' Delete Policy '
      description: Deletes the specified managed policy
      operationId: deletePolicy
      parameters:
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy you want to
          delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - policies
definitions: []
x-collection-name: AWS Identity and Access Management
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