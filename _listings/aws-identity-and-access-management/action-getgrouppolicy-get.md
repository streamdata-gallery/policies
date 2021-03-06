---
swagger: "2.0"
info:
  title: AWS Identity and Access Management API Get Group Policy
  version: 1.0.0
  description: |-
    Retrieves the specified inline policy document that is embedded in the specified IAM
          group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetGroupPolicy:
    get:
      summary: ' Get Group Policy '
      description: |-
        Retrieves the specified inline policy document that is embedded in the specified IAM
              group
      operationId: getGroupPolicy
      parameters:
      - in: query
        name: GroupName
        description: The name of the group the policy is associated with
        type: string
      - in: query
        name: PolicyName
        description: The name of the policy document to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - group policies
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