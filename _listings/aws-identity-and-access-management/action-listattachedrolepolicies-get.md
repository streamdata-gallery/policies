---
swagger: "2.0"
info:
  title: AWS Identity and Access Management API List Attached Role Policies
  version: 1.0.0
  description: Lists all managed policies that are attached to the specified IAM role.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListAttachedRolePolicies:
    get:
      summary: ' List Attached Role Policies '
      description: Lists all managed policies that are attached to the specified IAM
        role
      operationId: listAttachedRolePolicies
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PathPrefix
        description: The path prefix for filtering the results
        type: string
      - in: query
        name: RoleName
        description: The name (friendly name, not ARN) of the role to list attached
          policies for
        type: string
      responses:
        200:
          description: OK
      tags:
      - attached role policies
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