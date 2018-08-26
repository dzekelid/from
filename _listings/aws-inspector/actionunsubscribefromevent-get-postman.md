{
  "info": {
    "name": "AWS Inspector API Unsubscribe From Event",
    "_postman_id": "372bd215-affb-4df0-b593-e36cba2410cc",
    "description": "Disables the process of sending Amazon Simple Notification Service (SNS)\n         notifications about a specified event to a specified SNS topic.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attributes To Findings",
      "item": [
        {
          "id": "489e1f40-0d9b-4d5c-8248-6e4f020b4668",
          "name": "addAttributesToFindings",
          "request": {
            "url": "http://example.com/api/?Action=AddAttributesToFindings?attributes=attributes&findingArns=findingArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Assigns attributes (key and value pairs) to the findings that are specified by the\n         ARNs of the findings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1cfcb6cf-1581-4630-bc08-471b1706d11c"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Targets",
      "item": [
        {
          "id": "807ea174-e813-45e8-bcbc-12f01948d906",
          "name": "createAssessmentTarget",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssessmentTarget?assessmentTargetName=assessmentTargetName&resourceGroupArn=resourceGroupArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new assessment target using the ARN of the resource group that is generated\n         by."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "525fc07b-3391-4c71-9f45-3c75f05ad6c2"
            }
          ]
        },
        {
          "id": "6157d2ba-bb56-4842-81d8-d80bfbe06370",
          "name": "deleteAssessmentTarget",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssessmentTarget?assessmentTargetArn=assessmentTargetArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the assessment target that is specified by the ARN of the assessment\n         target."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47b7fd48-47a3-4fc7-a1d1-548e60ecdc7a"
            }
          ]
        },
        {
          "id": "a54ab34a-bf23-495d-a3a1-7a3a11df62fd",
          "name": "describeAssessmentTargets",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssessmentTargets?assessmentTargetArns=assessmentTargetArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the assessment targets that are specified by the ARNs of the assessment\n         targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "340d1e8d-5f29-42e1-955a-8e570ff0c58f"
            }
          ]
        },
        {
          "id": "32e685a6-8b16-4068-91b4-a059e3c4eb81",
          "name": "listAssessmentTargets",
          "request": {
            "url": "http://example.com/api/?Action=ListAssessmentTargets?filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the ARNs of the assessment targets within this AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4216637b-a54c-45eb-bea2-ab63d4d5133e"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Templates",
      "item": [
        {
          "id": "3c875aae-e0ec-42e7-ab44-04f02a55355c",
          "name": "createAssessmentTemplate",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssessmentTemplate?assessmentTargetArn=assessmentTargetArn&assessmentTemplateName=assessmentTemplateName&durationInSeconds=durationInSeconds&rulesPackageArns=rulesPackageArns&userAttributesForFindings=userAttributesForFindings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an assessment template for the assessment target that is specified by the ARN\n         of the assessment target."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f50c766-6167-4fa3-8938-cc22428833aa"
            }
          ]
        },
        {
          "id": "1fa2a184-11b3-461e-9653-1ba9b71c61e1",
          "name": "deleteAssessmentTemplate",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssessmentTemplate?assessmentTemplateArn=assessmentTemplateArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the assessment template that is specified by the ARN of the assessment\n         template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc8c5a12-4294-40ad-8ef6-dddc2a9df37b"
            }
          ]
        },
        {
          "id": "049136d0-9a16-43bf-a779-f0a956880e27",
          "name": "describeAssessmentTemplates",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssessmentTemplates?assessmentTemplateArns=assessmentTemplateArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the assessment templates that are specified by the ARNs of the assessment\n         templates."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77a088f4-a5d5-4172-a35d-66d4f8d10fea"
            }
          ]
        },
        {
          "id": "ac0b170f-7176-4166-8b39-1b146a30afb8",
          "name": "listAssessmentTemplates",
          "request": {
            "url": "http://example.com/api/?Action=ListAssessmentTemplates?assessmentTargetArns=assessmentTargetArns&filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the assessment templates that correspond to the assessment targets that are\n         specified by the ARNs of the assessment targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a1fa271-dcc7-4440-b12e-8eb35f75c56f"
            }
          ]
        }
      ]
    },
    {
      "name": "Resource Groups",
      "item": [
        {
          "id": "d04e5fb4-2591-4915-a96c-4991a2730676",
          "name": "createResourceGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateResourceGroup?resourceGroupTags=resourceGroupTags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a resource group using the specified set of tags (key and value pairs) that\n         are used to select the EC2 instances to be included in an Amazon Inspector assessment\n         target."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9d59f4f-2a9e-4984-9562-bdedc8c71ca7"
            }
          ]
        },
        {
          "id": "b589b654-773a-4c57-a413-0fbb793a700f",
          "name": "describeResourceGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeResourceGroups?resourceGroupArns=resourceGroupArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the resource groups that are specified by the ARNs of the resource\n         groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5662a4b-e0c2-4822-8d5d-966dd5e7be52"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Runs",
      "item": [
        {
          "id": "6d057ba5-6680-4551-a02e-df1adeb1dcbd",
          "name": "deleteAssessmentRun",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssessmentRun?assessmentRunArn=assessmentRunArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the assessment run that is specified by the ARN of the assessment\n         run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "912067cb-de24-446c-941b-51e6321177e7"
            }
          ]
        },
        {
          "id": "829e0e8c-9112-45f5-9c59-dbc892c36419",
          "name": "describeAssessmentRuns",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssessmentRuns?assessmentRunArns=assessmentRunArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the assessment runs that are specified by the ARNs of the assessment\n         runs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2523e19-db98-4d6e-a9ba-75b250fbbac1"
            }
          ]
        },
        {
          "id": "310d6dcb-4bee-4988-8df6-8b8f2e98c54e",
          "name": "listAssessmentRuns",
          "request": {
            "url": "http://example.com/api/?Action=ListAssessmentRuns?assessmentTemplateArns=assessmentTemplateArns&filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the assessment runs that correspond to the assessment templates that are\n         specified by the ARNs of the assessment templates."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0290520b-d3ea-4bfc-b3c0-0ed4e77f1fc4"
            }
          ]
        },
        {
          "id": "9436bcdb-68cd-43cc-8494-4269ec519803",
          "name": "startAssessmentRun",
          "request": {
            "url": "http://example.com/api/?Action=StartAssessmentRun?assessmentRunName=assessmentRunName&assessmentTemplateArn=assessmentTemplateArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Starts the assessment run specified by the ARN of the assessment template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d28e0ac9-da19-4147-937b-bf2e9393a90e"
            }
          ]
        },
        {
          "id": "b29aa9bc-eef7-400e-85b7-35a316d5b2c1",
          "name": "stopAssessmentRun",
          "request": {
            "url": "http://example.com/api/?Action=StopAssessmentRun?assessmentRunArn=assessmentRunArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Stops the assessment run that is specified by the ARN of the assessment\n         run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8669d5a4-8c2d-4c25-8b3d-996930925399"
            }
          ]
        }
      ]
    },
    {
      "name": "Cross Account Access Roles",
      "item": [
        {
          "id": "c922c8c7-2e3f-4d58-979e-c72a7f51986a",
          "name": "describeCrossAccountAccessRole",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCrossAccountAccessRole?registeredAt=registeredAt&roleArn=roleArn&valid=valid",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the IAM role that enables Amazon Inspector to access your AWS\n         account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f576a8d8-032e-4476-9513-dafedc249f7d"
            }
          ]
        },
        {
          "id": "a9161093-7e48-4e83-a3cb-627676d5dce8",
          "name": "registerCrossAccountAccessRole",
          "request": {
            "url": "http://example.com/api/?Action=RegisterCrossAccountAccessRole?roleArn=roleArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers the IAM role that Amazon Inspector uses to list your EC2 instances at the\n         start of the assessment run or when you call the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5931c959-54be-45d6-9a56-5a3aca9992d6"
            }
          ]
        }
      ]
    },
    {
      "name": "Findings",
      "item": [
        {
          "id": "9c3eb3fb-bfc2-4f3e-becb-847895dea1e7",
          "name": "describeFindings",
          "request": {
            "url": "http://example.com/api/?Action=DescribeFindings?findingArns=findingArns&locale=locale",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the findings that are specified by the ARNs of the findings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e701a083-5202-4c5f-a3dc-6321b9da5896"
            }
          ]
        },
        {
          "id": "56ede06e-b133-4415-aa77-ab4f2536143a",
          "name": "listFindings",
          "request": {
            "url": "http://example.com/api/?Action=ListFindings?assessmentRunArns=assessmentRunArns&filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists findings that are generated by the assessment runs that are specified by the\n         ARNs of the assessment runs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bfb91c13-4241-4d50-beb2-d55996af4366"
            }
          ]
        }
      ]
    },
    {
      "name": "Rules Packages",
      "item": [
        {
          "id": "bed931d9-2162-4395-8cce-11875ee18fc9",
          "name": "describeRulesPackages",
          "request": {
            "url": "http://example.com/api/?Action=DescribeRulesPackages?locale=locale&rulesPackageArns=rulesPackageArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the rules packages that are specified by the ARNs of the rules\n         packages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e51eeb1-48a9-4241-a514-243a6f4f0ba5"
            }
          ]
        },
        {
          "id": "66afb81a-9858-4bf3-b27e-593b6bbd8cdf",
          "name": "listRulesPackages",
          "request": {
            "url": "http://example.com/api/?Action=ListRulesPackages?maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all available Amazon Inspector rules packages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5b32dd9-5c69-4b53-aead-2006314a0ba9"
            }
          ]
        }
      ]
    },
    {
      "name": "Telemetry Metadata",
      "item": [
        {
          "id": "0553b3e6-ebbd-42ff-b157-1f1e1cafb119",
          "name": "getTelemetryMetadata",
          "request": {
            "url": "http://example.com/api/?Action=GetTelemetryMetadata?assessmentRunArn=assessmentRunArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Information about the data that is collected for the specified assessment\n         run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3909f99c-56c9-4563-89d3-06499079eb01"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Run Agents",
      "item": [
        {
          "id": "90f2b092-827e-49eb-935c-f0168444eb11",
          "name": "listAssessmentRunAgents",
          "request": {
            "url": "http://example.com/api/?Action=ListAssessmentRunAgents?assessmentRunArn=assessmentRunArn&filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the agents of the assessment runs that are specified by the ARNs of the\n         assessment runs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "370ecf27-ee56-4915-91b5-030c81ecf97f"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Subscriptions",
      "item": [
        {
          "id": "5c7f064c-102c-4aad-9d8d-3f520f872b34",
          "name": "listEventSubscriptions",
          "request": {
            "url": "http://example.com/api/?Action=ListEventSubscriptions?maxResults=maxResults&nextToken=nextToken&resourceArn=resourceArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the event subscriptions for the assessment template that is specified by\n         the ARN of the assessment template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7cf2eb1-f184-4a72-b088-04663cf20fd6"
            }
          ]
        },
        {
          "id": "582ce714-2ff6-4200-9e11-2efb368090bf",
          "name": "subscribeToEvent",
          "request": {
            "url": "http://example.com/api/?Action=SubscribeToEvent?event=event&resourceArn=resourceArn&topicArn=topicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables the process of sending Amazon Simple Notification Service (SNS) notifications\n         about a specified event to a specified SNS topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df69b718-c724-4775-813a-c8bd869793cc"
            }
          ]
        },
        {
          "id": "40f4504a-d73f-406d-871c-db98521db6d4",
          "name": "unsubscribeFromEvent",
          "request": {
            "url": "http://example.com/api/?Action=UnsubscribeFromEvent?event=event&resourceArn=resourceArn&topicArn=topicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables the process of sending Amazon Simple Notification Service (SNS)\n         notifications about a specified event to a specified SNS topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "daa5606f-13cf-4710-a758-04f3241f58e3"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags For Resources",
      "item": [
        {
          "id": "08c00f55-80b7-46a4-865c-cc120d3ba131",
          "name": "listTagsForResource",
          "request": {
            "url": "http://example.com/api/?Action=ListTagsForResource?resourceArn=resourceArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all tags associated with an assessment template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "441a7145-8a6a-409f-9629-ca3b420b6bb9"
            }
          ]
        },
        {
          "id": "1c053d8c-ad68-4440-adbb-ba57622a693e",
          "name": "setTagsForResource",
          "request": {
            "url": "http://example.com/api/?Action=SetTagsForResource?resourceArn=resourceArn&tags=tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets tags (key and value pairs) to the assessment template that is specified by the\n         ARN of the assessment template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2494e08-2a25-4fcf-820e-8a27cd1df79d"
            }
          ]
        }
      ]
    },
    {
      "name": "Agents",
      "item": [
        {
          "id": "8ee66399-066c-4c2f-a3cc-5f3cb94a6bfa",
          "name": "previewAgents",
          "request": {
            "url": "http://example.com/api/?Action=PreviewAgents?maxResults=maxResults&nextToken=nextToken&previewAgentsArn=previewAgentsArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Previews the agents installed on the EC2 instances that are part of the specified\n         assessment target."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94503609-a432-4864-ad4e-471b96503f2a"
            }
          ]
        }
      ]
    },
    {
      "name": "Attributes From Findings",
      "item": [
        {
          "id": "08c56cbf-5338-4e42-8815-a807589cef27",
          "name": "removeAttributesFromFindings",
          "request": {
            "url": "http://example.com/api/?Action=RemoveAttributesFromFindings?attributeKeys=attributeKeys&findingArns=findingArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes entire attributes (key and value pairs) from the findings that are specified\n         by the ARNs of the findings where an attribute with the specified key exists."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "763fca66-7a4d-447c-8ae3-881985ffe9e1"
            }
          ]
        }
      ]
    }
  ]
}