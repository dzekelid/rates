swagger: "2.0"
x-collection-name: AXA Assistance
x-complete: 1
info:
  title: AXA Assistance
  description: axa-assistance-is-a-worldwide-specialist-for-car-insurance-travel-health-and-home-services--trust-in-axa-assistance-for-your-insurance
  version: 1.0.0
host: sandbox.api.axa-assistance.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/vexp/roadside/assignments/{assignment_id}/rate:
    post:
      summary: Rates an assignment.
      description: Rates an assignment.
      operationId: postServiceVexpRoadsideAssignmentsAssignment_idRate
      x-api-path-slug: servicevexproadsideassignmentsassignment-idrate-post
      parameters:
      - in: path
        name: assignment_id
        description: Assignment unique identifier
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Ratesassignment.