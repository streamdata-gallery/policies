---
swagger: "2.0"
info:
  title: AWS Auto Scaling API Delete Policy
  version: 1.0.0
  description: Deletes the specified Auto Scaling policy.
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
      description: Deletes the specified Auto Scaling policy
      operationId: deletePolicy
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: PolicyName
        description: The name or Amazon Resource Name (ARN) of the policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - policies
definitions: []
x-collection-name: AWS Auto Scaling
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