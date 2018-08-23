{
  "info": {
    "name": "AWS S3 PUT Bucket lifecycle",
    "_postman_id": "61cfd36a-ca91-4283-bbac-329cab801f87",
    "description": "Creates a new lifecycle configuration for the bucket or replaces an existing lifecycle configuration",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bucket",
      "item": [
        {
          "id": "62acb9e7-8ef1-477b-b16e-8c1bd178c704",
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
              "id": "88670369-e720-43fa-9b89-bcb63679a9a0"
            }
          ]
        },
        {
          "id": "41c6c129-c17c-4b8a-9443-29804458e31d",
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
              "id": "7db86b4c-84dc-48d7-8b3e-ca8973360534"
            }
          ]
        },
        {
          "id": "704e0d3d-089b-4b2c-9fa0-0ab218104b72",
          "name": "get-bucket-accelerate",
          "request": {
            "url": "{{default}}/?accelerate",
            "method": "GET",
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
            "description": "This implementation of the GET operation uses the acceleratesubresource to return the Transfer Acceleration state of a bucket, which is eitherEnabled or Suspended"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ce7a616-0439-4faa-aa05-690b45197cc2"
            }
          ]
        },
        {
          "id": "6e39ca88-3bce-46b8-91a3-6d54a1dbec3a",
          "name": "put-bucket-accelerate",
          "request": {
            "url": "{{default}}/?accelerate",
            "method": "PUT",
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
            "description": "This implementation of the PUT operation uses the acceleratesubresource to set the Transfer Acceleration state of an existing bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "de31287a-731e-4d39-8b09-ae9e7654f00a"
            }
          ]
        },
        {
          "id": "8d50ae03-769a-4b1b-b5c6-19af276d75dc",
          "name": "get-bucket-acl",
          "request": {
            "url": "{{default}}/?acl",
            "method": "GET",
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
            "description": "This implementation of the GET operation uses the aclsubresource to return the access control list (ACL) of a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e604ff1a-06d1-4e54-b9b4-307c945b008e"
            }
          ]
        },
        {
          "id": "ffa054a4-676c-4679-9b28-eab991ce2d26",
          "name": "put-bucket-acl",
          "request": {
            "url": "{{default}}/?acl",
            "method": "PUT",
            "header": [
              {
                "key": "x-amz-acl",
                "value": "{}",
                "description": "Sets the ACL of the bucket using the specified canned ACL",
                "disabled": false
              },
              {
                "key": "x-amz-grant-full-control",
                "value": "{}",
                "description": "Allows the specified grantee(s) the READ, WRITE, READ_ACP, and WRITE_ACPtttttttttpermissions on the bucket",
                "disabled": false
              },
              {
                "key": "x-amz-grant-read",
                "value": "{}",
                "description": "Allows the specified grantee(s) to list the objects in the bucket",
                "disabled": false
              },
              {
                "key": "x-amz-grant-read-acp",
                "value": "{}",
                "description": "Allows the specified grantee(s) to read the bucket ACL",
                "disabled": false
              },
              {
                "key": "x-amz-grant-write",
                "value": "{}",
                "description": "Allows the specified grantee(s) to create, overwrite, and delete any object in thetttttttttbucket",
                "disabled": false
              },
              {
                "key": "x-amz-grant-write-acp",
                "value": "{}",
                "description": "Allows the specified grantee(s) to write the ACL for the applicabletttttttttbucket",
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
            "description": "This implementation of the PUT operation uses the aclsubresource to set the permissions on an existing bucket using access control lists(ACL)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ac16a9a-0bca-48ce-bc66-b3ea6a369252"
            }
          ]
        },
        {
          "id": "ce1f3ec7-87a6-4110-9bbd-b94120d7ece0",
          "name": "get-bucket-analytics-configuration",
          "request": {
            "url": "{{default}}/?analytics&amp;id=analytics-configuration-ID",
            "method": "GET",
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
            "description": "This implementation of the GET operation returns an analytics configuration (identified bythe analytics configuration ID) from the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ac112bb-d969-4918-94f6-bad425fa6947"
            }
          ]
        },
        {
          "id": "59dc5b36-2fbf-4501-8a85-527ff2117590",
          "name": "delete-bucket-analyticsconfiguration",
          "request": {
            "url": "{{default}}/?analytics&amp;id=analytics-configuration-ID?id=%7B%7D",
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
            "description": "This implementation of the DELETE operation deletes an analytics configuration(identified by the analytics configuration ID) from the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d3d196b-f5c2-4e5f-b59f-f4c877df5fa9"
            }
          ]
        },
        {
          "id": "2d03ec86-9880-4574-8755-e6a830e00934",
          "name": "put-bucket-analytics-configuration",
          "request": {
            "url": "{{default}}/?analytics&amp;id=configuration-ID",
            "method": "PUT",
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
            "description": "This implementation of the PUT operation adds an analytics configuration(identified by the analytics ID) to the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3051b74-6343-4167-84d6-89b20a04d93e"
            }
          ]
        },
        {
          "id": "48795d32-fe2d-4614-9c32-1fecf0747ce5",
          "name": "get-bucket-cors",
          "request": {
            "url": "{{default}}/?cors",
            "method": "GET",
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
            "description": "Returns the cors configuration information set for thebucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c2cb21e-910c-49fe-953e-64417bd6fe38"
            }
          ]
        },
        {
          "id": "5cb6dcc4-4f9b-44ff-a18f-807b6fb3779d",
          "name": "delete-bucket-cors",
          "request": {
            "url": "{{default}}/?cors",
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
            "description": "Deletes the cors configuration information set for the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1953aed-19a9-4517-acf2-eb5e7a43f62b"
            }
          ]
        },
        {
          "id": "7d304e56-f45d-440d-8e4a-a4fa27cfaa3b",
          "name": "put-bucket-inventory-configuration",
          "request": {
            "url": "{{default}}/?inventory&amp;id=configuration-ID",
            "method": "PUT",
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
            "description": "This implementation of the PUT operation adds an inventory configuration(identified by the inventory ID) to the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0400285f-63c7-410e-bd6e-8b63069a8229"
            }
          ]
        },
        {
          "id": "1a370ae0-7116-4ccf-ab0c-6b6c912caa5d",
          "name": "get-bucket-inventory-configuration",
          "request": {
            "url": "{{default}}/?inventory&amp;id=inventory-configuration-ID",
            "method": "GET",
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
            "description": "This implementation of the GET operation returns an inventory configuration (identified bythe inventory configuration ID) from the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1343cba-b4d0-4ec1-93fc-42b9ba9ab203"
            }
          ]
        },
        {
          "id": "2f157b57-0ef2-4ec0-9589-d94f995f66f1",
          "name": "delete-bucket-inventoryconfiguration",
          "request": {
            "url": "{{default}}/?inventory&amp;id=inventory-configuration-ID?id=%7B%7D",
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
            "description": "This implementation of the DELETE operation deletes an inventory configuration(identified by the inventory configuration ID) from the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd07644e-6160-42f1-91d3-5a555d0f3d58"
            }
          ]
        },
        {
          "id": "e93db950-3e6b-453c-8446-fbb41f01c5ec",
          "name": "get-bucket-lifecycle",
          "request": {
            "url": "{{default}}/?lifecycle",
            "method": "GET",
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
            "description": "NoteBucket lifecycle configuration now supports specifying lifecycle rule usingobject key name prefix, one or more object tags, or combination of both"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "462939d0-9e82-485a-ba79-57ad31531a2e"
            }
          ]
        },
        {
          "id": "cb796101-7fd8-4b89-b53c-fed6128facfa",
          "name": "put-bucket-lifecycle",
          "request": {
            "url": "{{default}}/?lifecycle",
            "method": "PUT",
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
            "description": "Creates a new lifecycle configuration for the bucket or replaces an existing lifecycle configuration"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c953c4c-6755-49ca-a648-8a66ef0615b7"
            }
          ]
        },
        {
          "id": "a80e3b8f-6dce-4ec5-bdb1-86e4e3422b7b",
          "name": "delete-bucket-lifecycle",
          "request": {
            "url": "{{default}}/?lifecycle",
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
            "description": "Deletes the lifecycle configuration from the specified bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9eab522-0f93-44ee-af1a-ff1aeb99a16a"
            }
          ]
        }
      ]
    },
    {
      "name": "Object",
      "item": [
        {
          "id": "498f7905-46f0-47e9-8d45-6c8fb8b1b286",
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
              "id": "422b933b-916c-4029-b344-eb2b26f54ede"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "0dfafc9a-11ca-4c4a-9d4a-803698703499",
          "name": "list-bucket-analytics-configurations",
          "request": {
            "url": "{{default}}/?analytics?ContinuationToken=%7B%7D",
            "method": "GET",
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
            "description": "This implementation of the GET operation returns a list of analyticsconfigurations for the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "642cdd72-1b75-428e-b16b-c3226cc0cd97"
            }
          ]
        },
        {
          "id": "ad1dca28-7055-4837-97d7-aff57268d33e",
          "name": "list-bucket-inventory-configurations",
          "request": {
            "url": "{{default}}/?inventory?ContinuationToken=%7B%7D",
            "method": "GET",
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
            "description": "This implementation of the GET operation returns a list of inventoryconfigurations for the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03e26681-4ed1-4d1a-b538-ffe208f4eb06"
            }
          ]
        }
      ]
    },
    {
      "name": "Multiple",
      "item": [
        {
          "id": "2929c872-0517-4c60-82e0-ec5e672cb3be",
          "name": "delete-multiple-objects",
          "request": {
            "url": "{{default}}/?delete",
            "method": "POST",
            "header": [
              {
                "key": "Content-Length",
                "value": "{}",
                "description": "Length of the body according to RFC 2616",
                "disabled": false
              },
              {
                "key": "Content-MD5",
                "value": "{}",
                "description": "The base64-encoded 128-bit MD5 digest of the data",
                "disabled": false
              },
              {
                "key": "x-amz-mfa",
                "value": "{}",
                "description": "The value is the concatenation of the authentication devices serial number, a space,tttttttttand the value that is displayed on your authenticationtttttttttdevice",
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
            "description": "The Multi-Object Delete operation enables you to delete multiple objects from a bucketusing a single HTTP request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4010a20a-3f8a-4ce0-9855-5941065d0d9d"
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