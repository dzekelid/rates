---
swagger: "2.0"
x-collection-name: YouTube
x-complete: 0
info:
  title: Youtube Add Videos Rate
  description: Add a like or dislike rating to a video or remove a rating from a video.
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: 1.0.0
host: www.googleapis.com
basePath: /youtube/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /videos/rate:
    post:
      summary: Add Videos Rate
      description: Add a like or dislike rating to a video or remove a rating from
        a video.
      operationId: postVeosRate
      x-api-path-slug: videosrate-post
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the YouTube video ID of the video
          that is being rated or having its rating removed
      - in: query
        name: rating
        description: Specifies the rating to record
      responses:
        200:
          description: OK
      tags:
      - Veos
      - Rate
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