{
  "info": {
    "name": "AWS S3 Complete Multipart Upload",
    "_postman_id": "0d82243d-0d0a-4505-98bb-0b5456053a10",
    "description": "This operation completes a multipart upload by assembling previously uploaded parts",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bucket",
      "item": [
        {
          "id": "6624fc7f-6e8d-43bc-99c1-0515cd855bed",
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
              "id": "96e838aa-f54f-4934-8206-d4cc75c33cc7"
            }
          ]
        },
        {
          "id": "f6c6b0dc-770b-47ef-9aef-d15acb3699c1",
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
              "id": "f90d8a50-f658-4f42-a420-67bd84c80db6"
            }
          ]
        },
        {
          "id": "c09a6d2d-bac9-4298-8c32-ef0c438f674a",
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
              "id": "03cbdf1f-ce77-49e7-862b-e6c38da1397e"
            }
          ]
        },
        {
          "id": "10cc999b-eacb-46f4-b607-baa2a2e745ab",
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
              "id": "4c1e2427-8541-48f2-8f20-ec8c8246af16"
            }
          ]
        },
        {
          "id": "911b8ebc-82e1-4d69-be1a-49f1f18fbe16",
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
              "id": "435afa9b-2042-4d63-b932-51d446701aeb"
            }
          ]
        },
        {
          "id": "c6d751d1-21c1-4e14-8fe9-2c93b7fb4105",
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
              "id": "e3402c83-4c50-4ee6-9bd8-b0c7bd655a33"
            }
          ]
        },
        {
          "id": "8df115ce-3a5c-4fdf-abe2-a737e69d9413",
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
              "id": "1ff82f78-0679-426d-8fb5-d342f4a4c729"
            }
          ]
        },
        {
          "id": "8fe672a9-a80d-42df-b4cc-c9667caca062",
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
              "id": "c9e4a117-f740-46db-83ff-f1177fe27d01"
            }
          ]
        },
        {
          "id": "2a53db34-a03a-4b9d-84a7-20ffb6119345",
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
              "id": "dff6b0b7-6eb8-4235-9812-7473a24f696c"
            }
          ]
        },
        {
          "id": "1b9979a6-988e-44db-8818-581c9eb2839d",
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
              "id": "f2af0a48-7812-48e6-8d6e-ca17dd8ef23a"
            }
          ]
        },
        {
          "id": "67322850-7e8a-48d0-9552-787b7a32873b",
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
              "id": "5ad1dc54-0dff-4d5d-96e1-94ce3ee4a908"
            }
          ]
        },
        {
          "id": "39262bda-873e-4049-bca3-de64e9d73059",
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
              "id": "2d2f4b48-79c6-4066-b948-c1615133d85b"
            }
          ]
        },
        {
          "id": "16a537f8-027d-431c-8c58-25cc26d9b9b9",
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
              "id": "c7bdcfb1-c283-4d06-9586-bc9d35e2602c"
            }
          ]
        },
        {
          "id": "78b9a64e-13c9-4133-82db-e900d7ff1d47",
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
              "id": "4e053566-5cba-4158-8fe0-c8de7b06360f"
            }
          ]
        },
        {
          "id": "91300ca4-8696-4d4d-bbda-b3680b5bc63e",
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
              "id": "a7e4ca2d-06dd-417d-8efa-e6fba334bbf3"
            }
          ]
        },
        {
          "id": "177aa187-95d1-47c0-86bf-6491d9fa687b",
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
              "id": "93fda003-9b99-4645-b730-6891094933dc"
            }
          ]
        },
        {
          "id": "78fa77cc-f86c-4dbd-9505-4bdf25f481bd",
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
              "id": "da93da5e-ce54-47c3-8f34-0b43d1d66982"
            }
          ]
        },
        {
          "id": "396aae1e-56d2-491d-ab43-9de718651c76",
          "name": "get-bucket-list-objects-version-2",
          "request": {
            "url": "{{default}}/?list-type=2?continuation-token=%7B%7D&delimiter=%7B%7D&encoding-type=%7B%7D&fetch-owner=%7B%7D&list-type=%7B%7D&max-keys=%7B%7D&prefix=%7B%7D&start-after=%7B%7D",
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
            "description": "This implementation of the GET operation returns some or all (up to 1,000) ofthe objects in a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca50dbb9-a353-46ca-bc34-14ca943fcde2"
            }
          ]
        },
        {
          "id": "fd4f39b0-3833-485e-af38-b661c7b5d70e",
          "name": "get-bucket-location",
          "request": {
            "url": "{{default}}/?location",
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
            "description": "This implementation of the GET operation uses thelocation subresource to return a bucket's region"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e33bd8bb-571f-45f8-beee-00a608bb6bb7"
            }
          ]
        },
        {
          "id": "71d94ed4-e687-42e4-a253-05f79599009a",
          "name": "get-bucket-logging",
          "request": {
            "url": "{{default}}/?logging",
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
            "description": "This implementation of the GET operation uses thelogging subresource to return the logging status of a bucketand the permissions users have to view and modify that status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46778fc0-1eab-4f36-b674-5364ade38402"
            }
          ]
        },
        {
          "id": "e00b1a3e-4b20-4971-88ba-8ffcc6e212a9",
          "name": "put-bucket-metrics",
          "request": {
            "url": "{{default}}/?metrics&amp;id=Id",
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
            "description": "Sets or updates a metrics configuration for the CloudWatch request metrics (specified by themetrics configuration ID) from the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d069e613-0716-4691-9ed2-947409cd760c"
            }
          ]
        },
        {
          "id": "8b075aad-8e0a-4632-8d0e-b3a64c0cc28d",
          "name": "delete-bucket-metrics",
          "request": {
            "url": "{{default}}/?metrics&amp;id=Id",
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
            "description": "Deletes a metrics configuration for the CloudWatch request metrics (specified by the metricsconfiguration ID) from the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf0c2efe-6578-4ad2-b351-1ffbe412307a"
            }
          ]
        },
        {
          "id": "107402bb-6e4f-4e74-80ff-ddb94c803270",
          "name": "get-bucket-metrics",
          "request": {
            "url": "{{default}}/?metrics&amp;id=id",
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
            "description": "Gets a metrics configuration for the CloudWatch request metrics (specified by the metricsconfiguration ID) from the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6f1976a-efd9-48e8-abe9-a6757e9a6026"
            }
          ]
        },
        {
          "id": "8403de15-4b39-4f9d-a2e6-c5480ee4649d",
          "name": "get-bucket-notification",
          "request": {
            "url": "{{default}}/?notification",
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
            "description": "This implementation of the GET operation uses thenotification subresource to return the notificationconfiguration of a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85950cfe-3118-4223-9577-1a7d87c1bebf"
            }
          ]
        },
        {
          "id": "552456be-f4df-4ddc-90e6-a0e7d9a0b26c",
          "name": "put-bucket-notification",
          "request": {
            "url": "{{default}}/?notification",
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
            "description": "The Amazon S3 notification feature enables you to receive notifications when certain eventshappen in your bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3074fa38-f925-473c-8ea4-5e695bd8ecd2"
            }
          ]
        },
        {
          "id": "061d4ed3-0ea2-45bf-9c9a-b8070a10ba66",
          "name": "get-bucket-policy",
          "request": {
            "url": "{{default}}/?policy",
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
            "description": "This implementation of the GET operation uses the policysubresource to return the policy of a specified bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3c5140f-b559-4cc4-97cf-18af38944069"
            }
          ]
        },
        {
          "id": "af55a17a-86c7-4fa3-8684-f999ee064174",
          "name": "put-bucket-policy",
          "request": {
            "url": "{{default}}/?policy",
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
            "description": "This implementation of the PUT operation uses the policysubresource to add to or replace a policy on a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38c54447-c537-41b8-8c46-a5ff19030ea5"
            }
          ]
        },
        {
          "id": "0e1d2d27-64e7-446f-818f-29e8e9857dd9",
          "name": "delete-bucket-policy",
          "request": {
            "url": "{{default}}/?policy",
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
            "description": "This implementation of the DELETE operation uses the policy subresource to delete the policy on a specified bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8dc577d-0fdf-40d2-81e9-187da289b39a"
            }
          ]
        },
        {
          "id": "2092a2b4-963e-4292-be46-c76e0d8790b1",
          "name": "get-bucket-replication",
          "request": {
            "url": "{{default}}/?replication?AWS Documentation &raquo; Amazon Simple Storage Service (S3) &raquo; API Reference &raquo; Operations on Buckets &raquo; GET Bucket replication=%7B%7D",
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
            "description": "Returns the replication configuration information set on the      bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "735d87c6-80a0-4c0c-8dd8-54057c27f832"
            }
          ]
        },
        {
          "id": "5e473e53-3ff0-497e-9687-2c8c7406c8af",
          "name": "put-bucket-replication",
          "request": {
            "url": "{{default}}/?replication?AWS Documentation &raquo; Amazon Simple Storage Service (S3) &raquo; API Reference &raquo; Operations on Buckets &raquo; PUT Bucket replication=%7B%7D",
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
            "description": "In a versioning-enabled bucket, this operation creates a new replication configuration (or      replaces an existing one, if present)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e73959b-4294-4983-8b07-63b7ed41d84c"
            }
          ]
        },
        {
          "id": "94e1eb10-8d2d-4725-aa50-0fa0d9643ad8",
          "name": "delete-bucket-replication",
          "request": {
            "url": "{{default}}/?replication",
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
            "description": "Deletes the replication subresource associated with the specified bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e089376-c64e-460e-84eb-128873d7cea0"
            }
          ]
        },
        {
          "id": "fda77ac2-158d-4371-9001-f775a352afae",
          "name": "get-bucket-tagging",
          "request": {
            "url": "{{default}}/?tagging",
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
            "description": "This implementation of the GET operation uses the taggingsubresource to return the tag set associated with the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94acbfa5-69bf-4d66-bc65-5487a8649b22"
            }
          ]
        },
        {
          "id": "2d1f0dbf-60d0-49cd-8a77-f86c899fe2db",
          "name": "put-bucket-tagging",
          "request": {
            "url": "{{default}}/?tagging",
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
            "description": "This implementation of the PUT operation uses the taggingsubresource to add a set of tags to an existing bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5311985-975f-4ff1-836b-63562a530e01"
            }
          ]
        },
        {
          "id": "9d05c667-27ab-4a56-a210-1ee90e56cff3",
          "name": "delete-bucket-tagging",
          "request": {
            "url": "{{default}}/?tagging",
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
            "description": "This implementation of the DELETE operation uses the taggingsubresource to remove a tag set from the specified bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e77273d-18f3-4d2d-9366-c94738c38f24"
            }
          ]
        },
        {
          "id": "bfc43cc4-53a9-4c93-a2b4-7ac77260aa41",
          "name": "get-bucket-versioning",
          "request": {
            "url": "{{default}}/?versioning",
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
            "description": "This implementation of the GET operation uses theversioning subresource to return the versioning state of abucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3998e6e6-e5a1-45c6-80c7-5f9d9233c058"
            }
          ]
        },
        {
          "id": "eac2fda4-9a41-4189-b1ea-62c811a5d529",
          "name": "put-bucket-versioning",
          "request": {
            "url": "{{default}}/?versioning",
            "method": "PUT",
            "header": [
              {
                "key": "x-amz-mfa",
                "value": "{}",
                "description": "The value is the concatenation of the authenticationtttttttttdevices serial number, a space, and the value displayed on yourtttttttttauthentication device",
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
            "description": "This implementation of the PUT operation uses theversioning subresource to set the versioning state of anexisting bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b29d11e9-3e8d-4034-ba11-5df3cb1d4c8f"
            }
          ]
        },
        {
          "id": "5353b302-0e40-417c-bad9-e80f35d74edd",
          "name": "get-bucket-object-versions",
          "request": {
            "url": "{{default}}/?versions?delimiter=%7B%7D&encoding-type=%7B%7D&key-marker=%7B%7D&max-keys=%7B%7D&prefix=%7B%7D&version-id-marker=%7B%7D",
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
            "description": "You can use the versions subresource to list metadata about all ofthe versions of objects in a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d97f94d0-59a8-4b8d-b896-2159a684b694"
            }
          ]
        },
        {
          "id": "00d07b42-e5c6-4281-8d7d-9abedf5b83a0",
          "name": "get-bucket-website",
          "request": {
            "url": "{{default}}/?website",
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
            "description": "This implementation of the GET operation returns the website configurationassociated with a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ed479ff-2c75-4204-9684-ac7c41599277"
            }
          ]
        },
        {
          "id": "e4afbd1c-2e78-4a4b-a306-b6b858e138a9",
          "name": "put-bucket-website",
          "request": {
            "url": "{{default}}/?website",
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
            "description": "Sets the configuration of the website that is specified in thewebsite subresource"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c581cb99-ab20-48f8-806d-c9d563d02422"
            }
          ]
        },
        {
          "id": "b8875bd7-ce9f-479a-9a5e-c3d0cb627605",
          "name": "delete-bucket-website",
          "request": {
            "url": "{{default}}/?website",
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
            "description": "This operation removes the website configuration for a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5ea399b-2472-4fd1-b814-4d5dfab71f8c"
            }
          ]
        }
      ]
    },
    {
      "name": "Object",
      "item": [
        {
          "id": "e7e21c07-8bf2-498b-a3c3-18be669eac3d",
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
              "id": "1ed5fcf8-0049-4b8c-8b1f-7130858f5fc1"
            }
          ]
        },
        {
          "id": "973ee3ff-1d89-43a9-b013-5f46dfc2e6bc",
          "name": "put-object--copy",
          "request": {
            "url": "{{default}}/destinationObject",
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
            "description": "This implementation of the PUT operation creates a copy of an object that is      already stored in Amazon S3"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9d91b3e-16f7-4960-b0cb-c2a34a8f1d58"
            }
          ]
        },
        {
          "id": "16a69610-53dd-4260-a799-7f80e8a5864c",
          "name": "get-object",
          "request": {
            "url": "{{default}}/ObjectName?response-cache-control=%7B%7D&response-content-disposition=%7B%7D&response-content-encoding=%7B%7D&response-content-language=%7B%7D&response-content-type=%7B%7D&response-expires=%7B%7D",
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
            "description": "This implementation of the GET operation retrieves objects from Amazon S3"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2da92548-38d9-4b3b-8ebf-e4f0341c21b7"
            }
          ]
        },
        {
          "id": "c23d06bc-51e0-4edc-a186-87c74da9e399",
          "name": "put-object",
          "request": {
            "url": "{{default}}/ObjectName",
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
            "description": "This implementation of the PUT operation adds an object to a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5fba25e1-f444-49bb-bf9d-0056298a80cc"
            }
          ]
        },
        {
          "id": "3b612442-9f1b-4fab-9b34-0c3edc55e4fe",
          "name": "delete-object",
          "request": {
            "url": "{{default}}/ObjectName",
            "method": "DELETE",
            "header": [
              {
                "key": "x-amz-mfa",
                "value": "{}",
                "description": "The value is the concatenation of the authenticationtttttttttdevices serial number, a space, and the value displayed on yourtttttttttauthentication device",
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
            "description": "The DELETE operation removes the null version (if there is one) of anobject and inserts a delete marker, which becomes the current version of the object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83031a9d-d1a7-41cd-bf11-4266f81bbf87"
            }
          ]
        },
        {
          "id": "0e7836cf-a095-4519-b828-6778d10452b5",
          "name": "get-object-acl",
          "request": {
            "url": "{{default}}/ObjectName?acl",
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
            "description": "This implementation of the GET operation uses the aclsubresource to return the access control list (ACL) of an object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c3911f6-0365-4e2d-ad1e-b25b43b26062"
            }
          ]
        },
        {
          "id": "5e5eb548-f700-4d61-81d7-b8bd2324b74d",
          "name": "put-object-acl",
          "request": {
            "url": "{{default}}/ObjectName?acl",
            "method": "PUT",
            "header": [
              {
                "key": "x-amz-acl",
                "value": "{}",
                "description": "Sets the ACL of the object using the specified canned ACL",
                "disabled": false
              },
              {
                "key": "x-amz-grant-full-control",
                "value": "{}",
                "description": "Allows the specified grantee the READ, WRITE, READ_ACP, andtttttttttWRITE_ACP permissions on the bucket",
                "disabled": false
              },
              {
                "key": "x-amz-grant-read",
                "value": "{}",
                "description": "Allows the specified grantee to list the objects in thetttttttttbucket",
                "disabled": false
              },
              {
                "key": "x-amz-grant-read-acp",
                "value": "{}",
                "description": "Allows the specified grantee to read the buckettttttttttACL",
                "disabled": false
              },
              {
                "key": "x-amz-grant-write",
                "value": "{}",
                "description": "Not applicable when granting access permissions on objects",
                "disabled": false
              },
              {
                "key": "x-amz-grant-write-acp",
                "value": "{}",
                "description": "Allows the specified grantee to write the ACL for thetttttttttapplicable bucket",
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
            "description": "This implementation of the PUT operation uses the aclsubresource to set the access control list (ACL) permissions for an object that alreadyexists in a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4dec896c-ea89-4058-a9c2-2e79664502e6"
            }
          ]
        },
        {
          "id": "a2d4236f-853b-4813-98e4-e4cff4aa6acf",
          "name": "post-object-restore",
          "request": {
            "url": "{{default}}/ObjectName?restore&amp;versionId=VersionID",
            "method": "POST",
            "header": [
              {
                "key": "Content-MD5",
                "value": "{}",
                "description": "The base64-encoded 128-bit MD5 digest of the data",
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
            "description": "Restores a temporary copy of an archived object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02d27f47-8c63-4e46-b338-af6d76fb2b07"
            }
          ]
        },
        {
          "id": "845dce7d-32a7-4a9e-9c18-71b0430158df",
          "name": "get-object-tagging",
          "request": {
            "url": "{{default}}/ObjectName?tagging",
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
            "description": "This implementation of the GET operation returns the tags associated with anobject"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6264dec-1645-4cf3-957b-193ec11388a9"
            }
          ]
        },
        {
          "id": "d0403672-bb4e-4fd8-a424-7a70849f42c5",
          "name": "put-object-tagging",
          "request": {
            "url": "{{default}}/ObjectName?tagging",
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
            "description": "This implementation of the PUT operation uses the taggingsubresource to add a set of tags to an existing object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22fa1cf4-f24f-4217-a904-7bbbd82c7426"
            }
          ]
        },
        {
          "id": "e6d8322b-5776-4590-be31-a64d38794381",
          "name": "get-object-torrent",
          "request": {
            "url": "{{default}}/ObjectName?torrent",
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
            "description": "This implementation of the GET operation uses thetorrent subresource to return torrent files from a bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aaa5b630-a118-49a8-b4bb-7391f9e0ffbd"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "c3c6ed5f-a0bb-412b-9e64-9ba19e5d3f3a",
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
              "id": "4ea9215d-0a66-4bf8-a0da-4a556def03a8"
            }
          ]
        },
        {
          "id": "ea3237a5-8b34-4f30-8998-1041a8a0c091",
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
              "id": "0aa70b02-be4c-4097-b40e-b819d527a3d1"
            }
          ]
        },
        {
          "id": "02404ac2-bcf4-4414-b9e0-f4dd06c2a2d6",
          "name": "list-bucket-metrics",
          "request": {
            "url": "{{default}}/?metrics?BucketName=%7B%7D&ContinuationToken=%7B%7D",
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
            "description": "Lists the metrics configurations for the CloudWatch request metrics of the bucket"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2739638-04b1-42b8-9a1a-2e68e3187b48"
            }
          ]
        },
        {
          "id": "6663d88c-99bc-43ba-a55e-b5c6df14bb35",
          "name": "list-multipart-uploads",
          "request": {
            "url": "{{default}}/?uploads?delimiter=%7B%7D&encoding-type=%7B%7D&key-marker=%7B%7D&max-uploads=%7B%7D&prefix=%7B%7D&upload-id-&#8203;marker=%7B%7D",
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
            "description": "This operation lists in-progress multipart uploads"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6eaafaf-4a24-4d67-bf97-1c553cc46048"
            }
          ]
        },
        {
          "id": "b6a4d800-4ef7-4c2a-a142-7083c60b2f9b",
          "name": "list-parts",
          "request": {
            "url": "{{default}}/ObjectName?uploadId=UploadId?encoding-type=%7B%7D&max-parts=%7B%7D&part-number&#8203;-marker=%7B%7D&uploadId=%7B%7D",
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
            "description": "This operation lists the parts that have been uploaded for a specific multipart upload"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab6f6526-4b8d-4b1d-bba4-a18779b2f5d2"
            }
          ]
        }
      ]
    },
    {
      "name": "Multiple",
      "item": [
        {
          "id": "b731d361-8f0e-40ee-9164-c47334a57ddd",
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
              "id": "f139e612-b8f2-49d5-b478-c6f807b6063f"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "0ea749ae-8eb9-46df-9bb8-8530fe31995e",
          "name": "upload-part",
          "request": {
            "url": "{{default}}/ObjectName?partNumber=PartNumber&amp;uploadId=UploadId?AWS Documentation &raquo; Amazon Simple Storage Service (S3) &raquo; API Reference &raquo; Operations on Objects &raquo; Upload Part - Copy=%7B%7D",
            "method": "PUT",
            "header": [
              {
                "key": "Content-Length",
                "value": "{}",
                "description": "The size of the part, in bytes",
                "disabled": false
              },
              {
                "key": "Content-MD5",
                "value": "{}",
                "description": "The base64-encoded 128-bit MD5 digest of the part data",
                "disabled": false
              },
              {
                "key": "Expect",
                "value": "{}",
                "description": "When your application uses 100-continue, it does not send the request body until ittttttttttreceives an acknowledgment",
                "disabled": false
              },
              {
                "key": "x-amz-copy-source",
                "value": "{}",
                "description": "The name of the source bucket and the source object key name separated by a                  slash (/)",
                "disabled": false
              },
              {
                "key": "x-amz-copy-source&#8203;-server-side&#8203;-encryption&#8203;-customer-algorithm",
                "value": "{}",
                "description": "Specifies algorithm to use when decrypting the source object",
                "disabled": false
              },
              {
                "key": "x-amz-copy-source&#8203;-server-side&#8203;-encryption&#8203;-customer-key",
                "value": "{}",
                "description": "Specifies the customer provided base-64 encoded encryption key for Amazon                      S3 to use to decrypt the source object",
                "disabled": false
              },
              {
                "key": "x-amz-copy-source-&#8203;server-side&#8203;-encryption&#8203;-customer-key-MD5",
                "value": "{}",
                "description": "Specifies the base64-encoded 128-bit MD5 digest of the encryption key                      according to RFC 1321",
                "disabled": false
              },
              {
                "key": "x-amz-copy-source-if-match",
                "value": "{}",
                "description": "Perform a copy if the source object entity tag (ETag) matches the specified                  value",
                "disabled": false
              },
              {
                "key": "x-amz-copy-source-if-modified-since",
                "value": "{}",
                "description": "Perform a copy if the source object is modified after the time specified                  using this header",
                "disabled": false
              },
              {
                "key": "x-amz-copy-source-if-none-match",
                "value": "{}",
                "description": "Perform a copy if the source object entity tag (ETag) is different than the                  value specified using this header",
                "disabled": false
              },
              {
                "key": "x-amz-copy-source-if-unmodified-since",
                "value": "{}",
                "description": "Perform a copy if the source object is not modified after the time                  specified using this header",
                "disabled": false
              },
              {
                "key": "x-amz-copy-source-range",
                "value": "{}",
                "description": "The range of bytes to copy from the source object",
                "disabled": false
              },
              {
                "key": "x-amz-server-side&#8203;-encryption&#8203;-customer-algorithm",
                "value": "{}",
                "description": "Specifies the algorithm to use to when encrypting the object",
                "disabled": false
              },
              {
                "key": "x-amz-server-side&#8203;-encryption&#8203;-customer-key",
                "value": "{}",
                "description": "Specifies the customer-provided base64-encoded encryption key for Amazon S3 to use intttttttttttttencrypting data",
                "disabled": false
              },
              {
                "key": "x-amz-server-side&#8203;-encryption&#8203;-customer-key-MD5",
                "value": "{}",
                "description": "Specifies the base64-encoded 128-bit MD5 digest of the encryption key according to RFC 1321",
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
            "description": "This operation uploads a part in a multipart upload"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9349c0eb-dfa4-416b-8b91-36a09378c708"
            }
          ]
        }
      ]
    },
    {
      "name": "Complete",
      "item": [
        {
          "id": "b09664a2-f455-4708-860d-e6b8cc6fbe9f",
          "name": "complete-multipart-upload",
          "request": {
            "url": "{{default}}/ObjectName?uploadId=UploadId",
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
            "description": "This operation completes a multipart upload by assembling previously uploaded parts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a142d64-c042-4465-b72f-1dd19269c8cd"
            }
          ]
        }
      ]
    },
    {
      "name": "Abort",
      "item": [
        {
          "id": "e9cda569-11ff-4efd-b205-6310dddce3a9",
          "name": "abort-multipart-upload",
          "request": {
            "url": "{{default}}/ObjectName?uploadId=UploadId",
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
            "description": "This operation aborts a multipart upload"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fd3dfd0d-5c74-4513-8e2c-bae49ce5cc7a"
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