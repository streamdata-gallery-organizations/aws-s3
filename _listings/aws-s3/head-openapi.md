---
swagger: "2.0"
x-collection-name: AWS S3
x-complete: 0
info:
  title: AWS S3 HEAD Bucket
  version: 1.0.0
  description: This operation is useful to determine if a bucket exists and you have
    permission to accessit
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:
    delete:
      summary: DELETE Bucket
      description: This implementation of the DELETE operation deletes the bucket
        named inthe URI
      operationId: delete-bucket
      x-api-path-slug: delete
      responses:
        200:
          description: OK
      tags:
      - Bucket
    head:
      summary: HEAD Bucket
      description: This operation is useful to determine if a bucket exists and you
        have permission to accessit
      operationId: head-bucket
      x-api-path-slug: head
      responses:
        200:
          description: OK
      tags:
      - Bucket
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