{
  "info": {
    "name": "AWS S3 DELETE Bucket",
    "_postman_id": "a3d8f858-3dd2-401d-a268-ca70da3c227c",
    "description": "This implementation of the DELETE operation deletes the bucket named inthe URI",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bucket",
      "item": [
        {
          "id": "f5b6e677-7841-4f54-aeae-d51c8c636df1",
          "name": "delete-bucket",
          "request": {
            "url": "{{default}}/",
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This implementation of the DELETE operation deletes the bucket named inthe URI"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "edfc053a-2735-4a19-ae0d-e60d02024974"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/"
    }
  ]
}