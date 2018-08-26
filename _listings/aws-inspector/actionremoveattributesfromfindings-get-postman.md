{
  "info": {
    "name": "AWS Inspector API Remove Attributes From Findings",
    "_postman_id": "f848a561-fce3-45fd-91ac-c8d49b57c596",
    "description": "Removes entire attributes (key and value pairs) from the findings that are specified\n         by the ARNs of the findings where an attribute with the specified key exists.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attributes To Findings",
      "item": [
        {
          "id": "81ef2ddc-0b17-4a90-a5d8-c110205057e0",
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
              "id": "feece9c9-f294-455a-835c-3e2989b45840"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Targets",
      "item": [
        {
          "id": "61abed7a-38d2-43dd-b6bc-7947f4a327c3",
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
              "id": "a9e6c475-80f1-4e0f-a505-c70a47f4b1d5"
            }
          ]
        },
        {
          "id": "2a948aa8-f415-43dc-ae69-052d05f756ed",
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
              "id": "b79c8b8b-5d18-43ee-aea9-3840e965eef5"
            }
          ]
        },
        {
          "id": "147e6e4c-c3d2-45bc-abe7-e5bb4fa63b62",
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
              "id": "3fbf2e62-3fb6-443d-a94e-28f90d587008"
            }
          ]
        },
        {
          "id": "6a9fc91b-9d50-4793-9e8b-b6973eebfbac",
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
              "id": "523e2f87-7b08-40c5-b35b-e4add9debdc9"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Templates",
      "item": [
        {
          "id": "70e398d3-e618-4c57-81ad-4004edcb8318",
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
              "id": "49af0eeb-ddae-495e-bc5c-f15f97eabff1"
            }
          ]
        },
        {
          "id": "dbdccd3b-5790-40c6-980a-ac9347487171",
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
              "id": "a6272de2-f463-4497-95cd-aec0dd9860bc"
            }
          ]
        },
        {
          "id": "b9d57c6f-585e-4bd1-966f-b5e853c85365",
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
              "id": "53ff9944-aef9-474c-9f4d-cb5c4fa7a414"
            }
          ]
        },
        {
          "id": "24527082-032e-41d6-a470-f39a2e4a12fd",
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
              "id": "bb4bfbe4-234a-47b9-af74-5503be0fc10b"
            }
          ]
        }
      ]
    },
    {
      "name": "Resource Groups",
      "item": [
        {
          "id": "daa13f28-f871-4911-9e5c-edfd1a072f09",
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
              "id": "e4a50b99-9e5d-4e33-9657-4a78c7f4e43d"
            }
          ]
        },
        {
          "id": "5024e2be-8320-43fc-8bb4-31ea45206cf6",
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
              "id": "394483be-2925-4042-939f-304f86358ca6"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Runs",
      "item": [
        {
          "id": "868eece3-445f-4326-81f3-90ee85763dcc",
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
              "id": "6c75b1a4-3613-4e57-a0f3-cdd68a3efe87"
            }
          ]
        },
        {
          "id": "5f60f554-1791-43cf-b26d-88bc36f8b8e6",
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
              "id": "bd4c63dc-e18e-409b-b625-66284d0cf856"
            }
          ]
        },
        {
          "id": "1731f676-ae85-4161-93e3-58c1e2a86c7e",
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
              "id": "b592ed90-7485-409f-af67-54dc7c67ded6"
            }
          ]
        }
      ]
    },
    {
      "name": "Cross Account Access Roles",
      "item": [
        {
          "id": "388c5cac-4578-42d7-b11e-a0e4be5b6490",
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
              "id": "e798391c-ffc4-4ee1-9a73-8159b784b8b2"
            }
          ]
        },
        {
          "id": "9a1ef284-d63a-49e1-ada7-76360207fae6",
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
              "id": "9ecba886-5081-41af-a9ee-3a0e0e97bb16"
            }
          ]
        }
      ]
    },
    {
      "name": "Findings",
      "item": [
        {
          "id": "4273d056-7edf-4f4e-9dde-3dbb4141ea0c",
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
              "id": "0c35d3fe-e745-4e1d-afdd-69d64bed042c"
            }
          ]
        },
        {
          "id": "93242949-a7bb-4d54-9d82-fb1da7565ba7",
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
              "id": "88986cfd-53f2-4c1c-85f3-f50267b4c56b"
            }
          ]
        }
      ]
    },
    {
      "name": "Rules Packages",
      "item": [
        {
          "id": "8fba0057-2fc2-4864-8873-3c9ec11c151f",
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
              "id": "67d3cfa3-ee1b-4edc-8fd3-42fdabb70cd5"
            }
          ]
        },
        {
          "id": "fee6ff4d-3705-4670-bd23-18987021700e",
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
              "id": "68630245-ffa5-4895-853c-0870123ca9cd"
            }
          ]
        }
      ]
    },
    {
      "name": "Telemetry Metadata",
      "item": [
        {
          "id": "c344ee94-b05b-4321-ae84-a35c381ee0f7",
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
              "id": "834f8f75-6e07-4d40-a7a8-ffab001e36bb"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Run Agents",
      "item": [
        {
          "id": "a6b45c7c-965e-42cc-8da9-e5e2bb04ef0d",
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
              "id": "0a8b1ff5-209e-4312-b559-7b1a9925cc21"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Subscriptions",
      "item": [
        {
          "id": "af9e1847-58c0-4e02-9855-ca9954d052be",
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
              "id": "1af8e4f1-5d28-4736-ba4a-15b39a96d07a"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags For Resources",
      "item": [
        {
          "id": "4816f4d7-44c4-4389-8267-25cbaf089b6a",
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
              "id": "c06801fd-7517-4871-886a-1a2a262318fe"
            }
          ]
        }
      ]
    },
    {
      "name": "Agents",
      "item": [
        {
          "id": "806d969a-bf01-4bc5-a1bb-8a280639fe77",
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
              "id": "a1b620ec-2e59-4708-bc03-a1cd09f3e781"
            }
          ]
        }
      ]
    },
    {
      "name": "Attributes From Findings",
      "item": [
        {
          "id": "fa00bc85-71a6-4125-811e-61cf9df9669b",
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
              "id": "950ed422-e5d1-4365-8d37-a171013c1a97"
            }
          ]
        }
      ]
    }
  ]
}