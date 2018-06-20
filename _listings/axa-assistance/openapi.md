---
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
  /service/v1/medical_consultations/{medical_consultation_id}/rate:
    post:
      summary: Rates a medical consultation
      description: Rates a medical consultation
      operationId: postServiceV1Medical_consultationsMedical_consultation_idRate
      x-api-path-slug: servicev1medical-consultationsmedical-consultation-idrate-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: medical_consultation_id
        description: ID of the medical consultation
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Ratesmedical
      - consultation
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
---