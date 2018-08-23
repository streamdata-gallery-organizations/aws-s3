{
  "info": {
    "name": "AWS S3 DELETE Object",
    "_postman_id": "6f32ea3b-f521-4dfe-af50-bd911d9dc33d",
    "description": "The DELETE operation removes the null version (if there is one) of anobject and inserts a delete marker, which becomes the current version of the object",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bucket",
      "item": [
        {
          "id": "be8dee5c-b685-4772-bdc5-b36cdf82d3f9",
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
              "id": "ec853c96-4b7a-4c76-9f7c-a28155865504"
            }
          ]
        },
        {
          "id": "098ce733-3fcd-496b-b793-3f6d520e4e60",
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
              "id": "c5def4b9-0acc-4334-bb3a-3e3b2b16204f"
            }
          ]
        },
        {
          "id": "55e6d4c3-7c64-4516-8e13-8e8cd7c16393",
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
              "id": "e4d4e6fc-3a8c-4d96-b1d9-97d00cbfe2a1"
            }
          ]
        },
        {
          "id": "84704949-5b4d-45e5-a444-65dc52fbaeb3",
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
              "id": "111135bb-c8e8-4770-a11f-41485faff045"
            }
          ]
        },
        {
          "id": "893ca37e-24b0-44e9-8990-b7e43dd61f4e",
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
              "id": "19e39fd0-8c41-4828-a800-7052102cf9c4"
            }
          ]
        },
        {
          "id": "145ba499-7ca0-415a-a279-0e6aa1aef8bd",
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
              "id": "e809a9df-deb5-4e7e-b7ed-bef24e20d67f"
            }
          ]
        },
        {
          "id": "cc52bef9-22bb-45f6-8460-d16bc443503f",
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
              "id": "65bf299a-ed41-4128-bacb-b209689e31e5"
            }
          ]
        },
        {
          "id": "c8395c9d-6a07-44dc-81e1-b54eb4cced42",
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
              "id": "4f61a907-580c-44f9-9ead-5e42bfcee852"
            }
          ]
        },
        {
          "id": "b1cb4e11-dc5e-47bc-bd6d-9f0539f42cbd",
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
              "id": "c0c95485-cc65-4a37-81d3-b118617b0f8f"
            }
          ]
        },
        {
          "id": "1dc48205-18b0-456e-a30d-e1130f5fe7a3",
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
              "id": "877697f6-633c-466f-9949-13f7ba917203"
            }
          ]
        },
        {
          "id": "952db37a-d851-426f-889b-e0c32ad7775f",
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
              "id": "5a2f3e60-bc3e-4b7e-af96-479175c51a07"
            }
          ]
        },
        {
          "id": "4258ceaf-50a9-4c0f-9d93-9eb6bbe31a9f",
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
              "id": "632fe7cd-5123-4494-9b3c-1eedc791fdd3"
            }
          ]
        },
        {
          "id": "2cb305aa-f8a2-48f7-ab3d-0fa658c884c4",
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
              "id": "762cbfbb-9836-4070-8bc4-df8d46dc8cf2"
            }
          ]
        },
        {
          "id": "2b1e905d-1b13-45a6-9fd3-5c495055b17b",
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
              "id": "1f65eadd-0951-4eb3-b20e-0de04fbecd28"
            }
          ]
        },
        {
          "id": "871c38c5-411d-4bc3-bde8-38a944296802",
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
              "id": "25dbce9c-0abb-4608-bd56-da085204164a"
            }
          ]
        },
        {
          "id": "97cb6c15-4752-4fc7-bce2-6dc17400e42f",
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
              "id": "9f22a41d-095c-4b43-b5d4-af113d7dd1cd"
            }
          ]
        },
        {
          "id": "e82ad5d6-dbe7-4f75-815f-007df4839b79",
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
              "id": "c131a1a9-8ce2-44a3-aea8-38301d70283e"
            }
          ]
        },
        {
          "id": "7a7e6099-b0f6-4d66-852f-b6172a28e208",
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
              "id": "47455e8c-e0a3-46ad-b140-8fcd020ecad9"
            }
          ]
        },
        {
          "id": "fcf06874-c665-4bd3-a45e-2938aee23176",
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
              "id": "0cbfe8d6-4a93-4ae3-8b20-a16fdd74bdfa"
            }
          ]
        },
        {
          "id": "f3096118-44ec-4dbe-bdb3-29f4a8a9101b",
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
              "id": "ff54b6dd-b50e-4caa-99bb-fb69e3700cbe"
            }
          ]
        },
        {
          "id": "ade13a8f-9b26-40ab-b868-18e2cce46b93",
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
              "id": "61029a18-377a-4f11-8283-f12a911de05f"
            }
          ]
        },
        {
          "id": "f2b6240d-541d-446f-90f1-13d563ef1db3",
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
              "id": "b049f9c2-ff16-41ac-9efe-06e07d7a6fa1"
            }
          ]
        },
        {
          "id": "bd95bd83-bdba-48d8-8a94-e84d396618df",
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
              "id": "7607658a-0d44-41fe-a992-52d4fb494a37"
            }
          ]
        },
        {
          "id": "a6f7539f-3a64-4c99-a65d-1077a13de4c3",
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
              "id": "3742740e-5c25-4442-9b2b-17a9b7f4fc71"
            }
          ]
        },
        {
          "id": "546bfcf5-f7fa-4cd7-a237-8dced02a81e3",
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
              "id": "0f507d99-ac46-45c8-b9c9-09aba7284ccb"
            }
          ]
        },
        {
          "id": "f9f07159-9501-4fce-848f-eb96b35cc016",
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
              "id": "6fba6731-cd4c-425c-b9ad-1bbe2efdac5f"
            }
          ]
        },
        {
          "id": "9a91b4f0-e9c6-4f69-847a-e8cb34205d62",
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
              "id": "ded29d94-e5bf-4fc9-8153-5821d9cd3c65"
            }
          ]
        },
        {
          "id": "e73f092c-0204-45ce-9ea7-1e9ff40a0ae6",
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
              "id": "a3cb94f0-9d2b-442c-96ac-626ceaf6e970"
            }
          ]
        },
        {
          "id": "93604921-1f0e-4ed3-b890-a39469e3a016",
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
              "id": "2ba2318b-5fcd-4eee-804c-fffa47212091"
            }
          ]
        },
        {
          "id": "df701c0f-43dc-4c90-8af0-1dbbad522e4b",
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
              "id": "b95e21e5-d498-4b77-8c9d-1b4b80a30fd0"
            }
          ]
        },
        {
          "id": "022bc098-204f-481a-8e4d-4ec8805585b1",
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
              "id": "430f1189-03fa-40b4-a299-e91d0cd2f01c"
            }
          ]
        },
        {
          "id": "30cff5a6-0ebd-40b8-8735-8194750f35e5",
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
              "id": "140f3749-c2bc-4cf8-a989-b75b73dfb462"
            }
          ]
        },
        {
          "id": "e95524b1-85bc-4865-9238-ec348cbe4b49",
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
              "id": "418648af-5aa8-4945-b4d7-b0fdc0ee2be9"
            }
          ]
        },
        {
          "id": "2a42df56-b6f9-47cc-b505-7d3d96ba959c",
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
              "id": "afbbf5d2-8550-45d3-a25c-1b31b8cedb01"
            }
          ]
        },
        {
          "id": "b9a4c494-6def-4f16-b727-7d33f0a55d23",
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
              "id": "1d9fecbd-0b2b-4c9c-8e4f-b6d37a47fc8c"
            }
          ]
        },
        {
          "id": "e8b17532-ddcb-4a9e-85bd-16883887a69b",
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
              "id": "4561775e-edeb-4949-a6c9-b2f38e820f1a"
            }
          ]
        },
        {
          "id": "0d85c313-2957-494c-9e36-ce7bee113b3b",
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
              "id": "e4d7518d-2332-4596-8af2-046febcd3e62"
            }
          ]
        },
        {
          "id": "0fd04bd7-cdaf-4f4f-9657-491e56611dfc",
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
              "id": "2cc760c8-2865-4c9b-b2e9-68334e43b715"
            }
          ]
        },
        {
          "id": "b45dd58f-011f-46e4-9aab-54c55b40eeb9",
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
              "id": "8f13d88a-9b88-40f5-ac33-9ebb6121a73a"
            }
          ]
        },
        {
          "id": "7d7cd360-29ca-4da9-87f0-6da5b0d45cbe",
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
              "id": "f2292ecf-2de0-4a00-a688-f4764a37c045"
            }
          ]
        }
      ]
    },
    {
      "name": "Object",
      "item": [
        {
          "id": "e867b150-5e9a-4cab-a719-11203d3e13db",
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
              "id": "6c144172-02ea-454b-b609-46ae07ab3065"
            }
          ]
        },
        {
          "id": "76a93a0b-88f4-479a-8545-2f766ee9bf52",
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
              "id": "361f7340-79a1-4a76-9e20-0018c33b5acc"
            }
          ]
        },
        {
          "id": "6eef5007-f9fd-47c5-9c3e-fe3c92f2dddd",
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
              "id": "2fc470ac-7078-4cd6-9942-f5d8d607f298"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "e3685ab1-9e72-4368-98ef-739f7e5cf5be",
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
              "id": "05eaccb9-8d4d-4290-aef3-fe4d6bd906ed"
            }
          ]
        },
        {
          "id": "bbb1f15c-22ef-4c2a-9e14-1e180cabf5fc",
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
              "id": "f283e0e2-ac64-4053-b00d-efc76e35bf15"
            }
          ]
        },
        {
          "id": "005e04f5-59d3-4e8d-b0e1-97f4d1978f30",
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
              "id": "150f958b-c455-4c1a-8b3f-c0be106e1113"
            }
          ]
        },
        {
          "id": "20839343-94d9-44ee-a38f-28397921094a",
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
              "id": "c719b198-1a89-4676-8369-1a43e8cf2c6b"
            }
          ]
        }
      ]
    },
    {
      "name": "Multiple",
      "item": [
        {
          "id": "ee17c35d-f490-400e-916b-b36148485517",
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
              "id": "eeef237a-d975-451b-8092-6e52da1c2ab0"
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