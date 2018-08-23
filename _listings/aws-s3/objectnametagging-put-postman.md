{
  "info": {
    "name": "AWS S3 PUT Object tagging",
    "_postman_id": "fd441f46-d46e-4748-ab3c-a590c3edce98",
    "description": "This implementation of the PUT operation uses the taggingsubresource to add a set of tags to an existing object",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bucket",
      "item": [
        {
          "id": "abcd95c4-d206-4921-8760-1a8344ebdba9",
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
              "id": "f363d4f7-2921-4501-86d6-7958c86e1f01"
            }
          ]
        },
        {
          "id": "1c15b192-e3d0-4070-a456-4e4258a63020",
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
              "id": "0c10bd91-b97d-4494-91ba-36fcfd068b20"
            }
          ]
        },
        {
          "id": "270ac8ad-3d69-44b9-afbb-974f732ca9df",
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
              "id": "ddf90e94-6b8b-42eb-b966-b33a4d2895c9"
            }
          ]
        },
        {
          "id": "1c7d78ae-2e17-4a28-920b-b9b24da2a428",
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
              "id": "3548e827-fc0a-49c7-b04e-49e3e98c34ba"
            }
          ]
        },
        {
          "id": "2d2ca4f0-fb44-4247-b23b-e9f4e5b8855c",
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
              "id": "89bc7d87-c8b7-4c8d-8c30-ba55ebd1b118"
            }
          ]
        },
        {
          "id": "03cdac44-43ed-4f01-910f-d17f92290254",
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
              "id": "fa64e3bd-641f-44bb-82f5-e6ae6113a5a0"
            }
          ]
        },
        {
          "id": "0c2d69f7-d6ff-4d7c-877e-01527e450722",
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
              "id": "d2bf2751-c268-44fc-9b41-fcfa7b23e8da"
            }
          ]
        },
        {
          "id": "bb817b88-7f1b-4d64-ab6c-87f7c605e81f",
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
              "id": "944af098-f1ef-4a4a-bb2b-b58f16c876fb"
            }
          ]
        },
        {
          "id": "8f3bf028-fa39-4f34-8670-9d44e63166ef",
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
              "id": "07717a9c-6312-4d8c-a706-cd2ebe4573a7"
            }
          ]
        },
        {
          "id": "c2aca904-ea81-4e50-8532-ba7872e92db4",
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
              "id": "2fad00c7-cbe0-48d3-a5af-bdebe6309e62"
            }
          ]
        },
        {
          "id": "c48ab480-03dd-4a82-aadf-d4d850b68a80",
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
              "id": "2b8ee554-a7ef-4ab2-94c3-5296f4f1cc93"
            }
          ]
        },
        {
          "id": "d534c268-b0e7-4a31-a0ca-c2f2db28e75f",
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
              "id": "39974b8f-aa01-455f-9d37-93f1697bdb05"
            }
          ]
        },
        {
          "id": "826049f4-f49c-45c2-981d-7b23e0c30d0c",
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
              "id": "f50af23c-3c73-467b-9ec6-14379cb6fc0d"
            }
          ]
        },
        {
          "id": "f3ffb07c-63b7-4e83-b025-df2c8235d02f",
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
              "id": "a1abf349-6f03-4053-8cfa-547672566c08"
            }
          ]
        },
        {
          "id": "5568d8a5-f3d7-4c02-ab5c-0deb038860be",
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
              "id": "6925f5d8-21b1-4fb5-b400-d55615d3ad20"
            }
          ]
        },
        {
          "id": "e76c1e29-a6f6-406c-aa16-a28115da85ec",
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
              "id": "ab802f8c-9689-4c45-8b86-101b3b5e0272"
            }
          ]
        },
        {
          "id": "3eb4a64c-3bcb-4c08-9449-f0af359546d2",
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
              "id": "24adfbd7-54db-47ba-b758-53492f68d07a"
            }
          ]
        },
        {
          "id": "22b05319-9940-42d1-be41-e271eee5e4e4",
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
              "id": "542228fd-a1c3-415b-b79a-24ea11e929d8"
            }
          ]
        },
        {
          "id": "79bfe46f-79b2-49ea-adf7-bc8d36810784",
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
              "id": "a2e25280-597f-47d8-9313-a3a425435812"
            }
          ]
        },
        {
          "id": "bd337117-9ce2-425f-93a4-0ce51e65b388",
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
              "id": "3ee1d96c-016c-4547-9efb-06fd26b3abfd"
            }
          ]
        },
        {
          "id": "cd49932c-2c51-4869-aec2-239c26fdd302",
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
              "id": "f3ee1bac-6614-4d55-8faf-b6dc7044de4a"
            }
          ]
        },
        {
          "id": "5b95d4cb-02f3-400e-bebd-275543786065",
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
              "id": "808b88d2-af39-48be-89f1-11a8a2717a88"
            }
          ]
        },
        {
          "id": "ff69217d-a1d7-494d-8364-a4f64488a7bc",
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
              "id": "e6564de4-5bdd-47bd-8b2f-315f8997895d"
            }
          ]
        },
        {
          "id": "e88d1f4f-b844-4c95-b08b-b9b0345c4919",
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
              "id": "793c1a7c-baa2-4ad6-ae61-20316ea9a4fa"
            }
          ]
        },
        {
          "id": "2dde9856-c23b-4632-ac25-9fe0bb4f165e",
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
              "id": "e5d43074-a849-4100-a2f3-07b9d73fc754"
            }
          ]
        },
        {
          "id": "dbc0dd3b-c543-4923-8dda-aef0d93edaea",
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
              "id": "a6235db0-bae7-4fe0-bff8-00d7a949970b"
            }
          ]
        },
        {
          "id": "0f9d3a2b-f658-4d8c-a6e2-50c064b6dfe0",
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
              "id": "cc098a32-8190-4494-aa6b-4a60c9bb411f"
            }
          ]
        },
        {
          "id": "25b81247-bf44-4e69-a906-ded6964f7207",
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
              "id": "ce044acc-e981-4d6d-81e7-da60fcbdde6c"
            }
          ]
        },
        {
          "id": "4a56d401-2249-45ae-8461-c716efbea759",
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
              "id": "2ed3f32a-c446-4100-b2e2-bf8830760098"
            }
          ]
        },
        {
          "id": "6497ac1f-3c67-4d3f-917f-a726ce7dda7e",
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
              "id": "48b4cf45-2315-4814-be3e-bbce70900277"
            }
          ]
        },
        {
          "id": "7afcf005-67f7-4061-bbee-9422f65af8ee",
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
              "id": "20ed4d08-3a6c-4b5a-b81b-4348585e9546"
            }
          ]
        },
        {
          "id": "68146495-b24b-4942-aa05-f98bc155cb50",
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
              "id": "eb29aa21-5dd9-4c2a-b4c5-4d26207b9f3c"
            }
          ]
        },
        {
          "id": "e6139263-85f6-4aae-b209-548029175c9c",
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
              "id": "faf0fe32-bd55-4a12-a865-c4d3dc0a5fa6"
            }
          ]
        },
        {
          "id": "b9a6f2d9-da12-49bc-93fc-77ad272b009f",
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
              "id": "d9286f3f-9d29-4652-9d1b-cc3aa412d459"
            }
          ]
        },
        {
          "id": "5337c180-1c2a-42a4-bd93-60ffea0bf178",
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
              "id": "7868e070-1d54-44fd-be60-21948f259427"
            }
          ]
        },
        {
          "id": "698f9e5c-a811-4375-99e1-35cbd8b54868",
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
              "id": "37103114-4d93-435b-b2ee-b6bb2cc8096e"
            }
          ]
        },
        {
          "id": "e4c20d87-b326-4122-b8db-51ae486e8ac3",
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
              "id": "8dcc801d-6e50-4539-b737-e6500bd2400d"
            }
          ]
        },
        {
          "id": "77163cce-1ff5-4f7e-85ab-9653e903fe14",
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
              "id": "891f8996-87a6-4be6-bc62-27ada1232948"
            }
          ]
        },
        {
          "id": "c3367fc2-add0-472e-a78d-050750c6309e",
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
              "id": "c3ed3ae4-aba9-478f-bd6a-1b3ace900f36"
            }
          ]
        },
        {
          "id": "786b9635-43b9-4936-bc9e-bab8045157b0",
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
              "id": "6b6346e7-fe9b-44ba-b9b4-93308482d771"
            }
          ]
        }
      ]
    },
    {
      "name": "Object",
      "item": [
        {
          "id": "a08122e3-5cbc-488b-8278-af03ca1adb91",
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
              "id": "e5f7f85e-17f9-44c4-88f9-f03ac671ce5b"
            }
          ]
        },
        {
          "id": "d8cdc542-79ae-4bdd-8726-af79d296caa9",
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
              "id": "6a4e1571-6f54-4d2f-b022-48aec09df9a1"
            }
          ]
        },
        {
          "id": "d34cba7f-8bc7-4839-b293-7919e460c0ca",
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
              "id": "27eab7c6-a1ec-49d2-93fb-d51fa9d8a7b0"
            }
          ]
        },
        {
          "id": "e6154a3a-3df4-4f91-908f-59f36083dde8",
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
              "id": "4d5c5114-5d7c-4003-9a68-adb182f1a382"
            }
          ]
        },
        {
          "id": "7b6be641-2cfb-4f6f-a887-c4eb77e506b1",
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
              "id": "e60f8dd5-217a-49ff-9277-b1e17af55e00"
            }
          ]
        },
        {
          "id": "e3d5e371-8ed0-4202-a3f3-d577aa567787",
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
              "id": "ae1af7ea-1f09-446d-b8e4-328f9b2eddfb"
            }
          ]
        },
        {
          "id": "05c5e6f7-7bcd-4210-a5ae-6b0a0d70d5ee",
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
              "id": "0b5b87de-e927-41f2-b423-ab1e751496f1"
            }
          ]
        },
        {
          "id": "7c14c57a-f266-48c1-a880-dedf2d3fcc26",
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
              "id": "ce7288cf-9c92-4df7-a1ef-64e2fedf9a38"
            }
          ]
        },
        {
          "id": "d431cee5-a453-455f-a17b-6d0da5c224a6",
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
              "id": "b0ef94f9-5584-445c-9f4c-008e6bfae829"
            }
          ]
        },
        {
          "id": "97ee2420-ae5d-45e5-af8c-4cfb074e8991",
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
              "id": "bd43ffca-d622-4d23-a950-124a3b4eb009"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "f4c12b17-5efc-4799-842e-e0ead8326455",
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
              "id": "00e01980-815e-4447-a44f-1b52741478ee"
            }
          ]
        },
        {
          "id": "63e50475-9b1f-48d2-99a2-46e69994ce51",
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
              "id": "72f857df-4bae-4f8a-b15c-7eb034b10102"
            }
          ]
        },
        {
          "id": "5c1deff0-6e67-45f7-8196-51e7ef1a7b28",
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
              "id": "895e6f00-95a0-490e-8906-06f93b41c4b6"
            }
          ]
        },
        {
          "id": "e9f32de8-c9e7-4809-9519-a4aef8537d7a",
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
              "id": "8df9c682-0034-4305-96fc-4e2e1f5d6b3d"
            }
          ]
        }
      ]
    },
    {
      "name": "Multiple",
      "item": [
        {
          "id": "090e03c1-cfa9-493d-abec-a79a1e745b97",
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
              "id": "3f62616d-f0ff-4a00-9fca-d44df29fb168"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "0fd021e8-cc1f-4830-a2dd-c8f65e3784bd",
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
              "id": "01f6a6e0-984b-4724-b2ae-1781faa0fd03"
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