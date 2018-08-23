{
  "info": {
    "name": "AWS S3 PUT Bucket",
    "_postman_id": "d9ef236b-3afa-47fa-93c5-23ec7b43966f",
    "description": "This implementation of the PUT operation creates a new bucket",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bucket",
      "item": [
        {
          "id": "051c5825-7f49-4c98-a430-73442ac2e8b9",
          "name": "put-bucket",
          "request": {
            "url": "{{default}}/",
            "method": "PUT",
            "header": [
              {
                "key": "x-amz-acl",
                "value": "{}",
                "description": "The canned ACL to apply to the bucket you are creating",
                "disabled": false
              },
              {
                "key": "x-amz-grant-full-control",
                "value": "{}",
                "description": "Allows grantee the READ, WRITE, READ_ACP, and WRITE_ACP permissions on thettttttttttttbucket",
                "disabled": false
              },
              {
                "key": "x-amz-grant-read",
                "value": "{}",
                "description": "Allows grantee to list the objects in the bucket",
                "disabled": false
              },
              {
                "key": "x-amz-grant-read-acp",
                "value": "{}",
                "description": "Allows grantee to read the bucket ACL",
                "disabled": false
              },
              {
                "key": "x-amz-grant-write",
                "value": "{}",
                "description": "Allows grantee to create, overwrite, and delete any object in the bucket",
                "disabled": false
              },
              {
                "key": "x-amz-grant-write-acp",
                "value": "{}",
                "description": "Allows grantee to write the ACL for the applicable bucket",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This implementation of the PUT operation creates a new bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "840ba12e-8c40-4bd5-b9aa-4f8e4ee62e33"
            }
          ]
        },
        {
          "id": "888e67bc-c089-4829-bec2-4caaba798d98",
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
              "id": "3609087d-c77c-4e78-b2d1-abf2a52efb17"
            }
          ]
        }
      ]
    },
    {
      "name": "Object",
      "item": [
        {
          "id": "583b6b31-78f5-4035-94b6-e344fb1c057c",
          "name": "post-object",
          "request": {
            "url": "{{default}}/",
            "method": "POST",
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
            "description": "The POST operation adds an object to a specified bucket using HTML forms"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75254290-e06a-40c8-8b52-73e6a576592f"
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