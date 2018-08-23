{
  "info": {
    "name": "AWS S3 HEAD Bucket",
    "_postman_id": "897b4163-b4ff-423a-8ef7-5f4395649d96",
    "description": "This operation is useful to determine if a bucket exists and you have permission to accessit",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bucket",
      "item": [
        {
          "id": "78073be7-7165-4b6a-afc4-bb01906a4bfa",
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
              "id": "1299eb50-4682-4031-9230-5d2761610e9f"
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