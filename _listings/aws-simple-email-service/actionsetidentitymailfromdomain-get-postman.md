{
  "info": {
    "name": "AWS Simple Email Service API Set Identity Mail From Domain",
    "_postman_id": "efc44fac-2105-4d3c-a35e-40c0e5b0767b",
    "description": "Enables or disables the custom MAIL FROM domain setup for a verified identity (an email address or a domain).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Receipt Rule Sets",
      "item": [
        {
          "id": "7f016270-cb67-487c-9e11-8606f01c9a3d",
          "name": "cloneReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=CloneReceiptRuleSet?OriginalRuleSetName=OriginalRuleSetName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a receipt rule set by cloning an existing one."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56ad3553-2ee8-491a-97c9-f6f76637e574"
            }
          ]
        },
        {
          "id": "61d30b01-3461-492c-8df9-a4ee25fa1980",
          "name": "createReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an empty receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8dedb9b6-b8ed-4072-84b1-6667d426a982"
            }
          ]
        },
        {
          "id": "f88e0e33-ba96-40f7-828b-db441b8c55bf",
          "name": "deleteReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified receipt rule set and all of the receipt rules it contains."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d4f47df-ee9c-4d83-9ed2-eb36078ffe13"
            }
          ]
        },
        {
          "id": "b58ad4a3-cd58-49f8-b8e5-88a6a45ab2cc",
          "name": "describeActiveReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeActiveReceiptRuleSet?Metadata=Metadata&Rules.member.N=Rules.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the metadata and receipt rules for the receipt rule set that is currently active."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dceddc5a-e5d2-45ab-b0fa-d6d2da51b011"
            }
          ]
        },
        {
          "id": "48070da4-4e30-4ebc-838a-f9689c09ad68",
          "name": "describeReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the details of the specified receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56714a26-bca8-4066-8114-bdd15617082d"
            }
          ]
        },
        {
          "id": "47592579-d578-45b8-b68a-45c2a288b5e5",
          "name": "listReceiptRuleSets",
          "request": {
            "url": "http://example.com/api/?Action=ListReceiptRuleSets?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the receipt rule sets that exist under your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76259dc6-a3d4-4774-97e7-1323e3a5fc1e"
            }
          ]
        },
        {
          "id": "22b601be-bd1f-4c41-a023-3b9b7809822c",
          "name": "reorderReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=ReorderReceiptRuleSet?RuleNames.member.N=RuleNames.member.N&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Reorders the receipt rules within a receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "983644cc-60c2-4794-95be-fc0e56d8b5e0"
            }
          ]
        },
        {
          "id": "98c87aa3-2dae-4ffc-be9d-6adbdfd80467",
          "name": "setActiveReceiptRuleSet",
          "request": {
            "url": "http://example.com/api/?Action=SetActiveReceiptRuleSet?RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the specified receipt rule set as the active receipt rule set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4e9b5bf-96e7-4e9d-b3cb-7dc6ad7d4a37"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Sets",
      "item": [
        {
          "id": "16d524ad-c485-40b9-9b2a-031394725060",
          "name": "createConfigurationSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateConfigurationSet?ConfigurationSet=ConfigurationSet",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e9f2c54-452c-4af2-a4d7-0b5aa624950d"
            }
          ]
        },
        {
          "id": "a6cfdc1b-569c-473b-90a6-9bef642cf727",
          "name": "deleteConfigurationSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConfigurationSet?ConfigurationSetName=ConfigurationSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0476cef1-4100-4092-bffa-f22b50427b08"
            }
          ]
        },
        {
          "id": "27246a08-e057-49a0-a5a0-00c4446505d3",
          "name": "describeConfigurationSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConfigurationSet?ConfigurationSetAttributeNames.member.N=ConfigurationSetAttributeNames.member.N&ConfigurationSetName=ConfigurationSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the details of the specified configuration set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed0bc40b-9f4a-46da-b91b-aa4d7742e135"
            }
          ]
        },
        {
          "id": "26160a91-0d99-4ed5-857b-af99e530c4ce",
          "name": "listConfigurationSets",
          "request": {
            "url": "http://example.com/api/?Action=ListConfigurationSets?MaxItems=MaxItems&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the configuration sets associated with your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d32da4df-4bde-4dc3-b248-aaf5e0a56b8a"
            }
          ]
        }
      ]
    },
    {
      "name": "Configuration Set Event Destination",
      "item": [
        {
          "id": "51d13b4c-f18a-4a83-83c2-466d8637ecbf",
          "name": "createConfigurationSetEventDestination",
          "request": {
            "url": "http://example.com/api/?Action=CreateConfigurationSetEventDestination?ConfigurationSetName=ConfigurationSetName&EventDestination=EventDestination",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a configuration set event destination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bcf5a63-80bc-4e5c-811b-8e3efc72b0d3"
            }
          ]
        },
        {
          "id": "849338fa-1d3d-4d88-bf19-b1f919475b31",
          "name": "deleteConfigurationSetEventDestination",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConfigurationSetEventDestination?ConfigurationSetName=ConfigurationSetName&EventDestinationName=EventDestinationName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a configuration set event destination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6046a78-4b6f-465c-ae1b-c5f6260a404d"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Filters",
      "item": [
        {
          "id": "d3125555-63be-407d-8e9e-4b589e1b0f42",
          "name": "createReceiptFilter",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptFilter?Filter=Filter",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new IP address filter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb02d5fc-970d-4937-a355-548634005b87"
            }
          ]
        },
        {
          "id": "03a3ecfb-37f4-45b8-ab95-93299d44ae97",
          "name": "deleteReceiptFilter",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptFilter?FilterName=FilterName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified IP address filter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39bbdb2e-85cb-4fda-9ee5-a62543c13fdc"
            }
          ]
        },
        {
          "id": "714f4517-cd5e-49ee-b164-01a7795e2093",
          "name": "listReceiptFilters",
          "request": {
            "url": "http://example.com/api/?Action=ListReceiptFilters?Filters.member.N=Filters.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the IP address filters associated with your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ceb6a29a-a405-4bdf-bca6-51c5ebf6b949"
            }
          ]
        }
      ]
    },
    {
      "name": "Receipt Rules",
      "item": [
        {
          "id": "36342011-1dda-4999-8e37-b0e5c6a2573c",
          "name": "createReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=CreateReceiptRule?After=After&Rule=Rule&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "980ed355-6dc1-496d-ab71-85cd890355ec"
            }
          ]
        },
        {
          "id": "25f62b0a-c974-40b8-b021-51c156b05db3",
          "name": "deleteReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReceiptRule?RuleName=RuleName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e78deca3-ffb5-4129-8573-2c9fbce2f725"
            }
          ]
        },
        {
          "id": "e760995c-346e-4803-b005-19a573fb63b4",
          "name": "describeReceiptRule",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReceiptRule?RuleName=RuleName&RuleSetName=RuleSetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the details of the specified receipt rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38c5e187-a08a-415f-9904-5ed3b5235540"
            }
          ]
        }
      ]
    },
    {
      "name": "Identity",
      "item": [
        {
          "id": "932d7072-5c72-486c-b023-fed43871c347",
          "name": "deleteIdentity",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIdentity?Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified identity (an email address or a domain) from the list of verified identities."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0602edf7-fc73-426f-ae2e-e9ed777a890f"
            }
          ]
        },
        {
          "id": "e1d5b776-1137-4676-abc3-e8a33f9b7f8b",
          "name": "deleteIdentityPolicy",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIdentityPolicy?Identity=Identity&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified sending authorization policy for the given identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "167ddd17-b1d9-4711-8095-a9ecce45b145"
            }
          ]
        },
        {
          "id": "7c720749-f69f-4f1b-a105-569edd7b2ddd",
          "name": "getIdentityDkimAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityDkimAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the current status of Easy DKIM signing for an entity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4617b7dd-fb9c-454e-b586-8bf722842850"
            }
          ]
        },
        {
          "id": "0e23742b-30c8-47ce-9e1f-040e44bafaa1",
          "name": "getIdentityMailFromDomainAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityMailFromDomainAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the custom MAIL FROM attributes for a list of identities (email addresses and/or domains)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f44b5507-e3b5-4786-961f-57d8b243bb1d"
            }
          ]
        },
        {
          "id": "8a3ef196-6d0d-4146-be56-a6625685609f",
          "name": "getIdentityNotificationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityNotificationAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a list of verified identities (email addresses and/or domains), returns a structure describing identity notification attributes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbc0f864-b49e-499f-b1d7-6af485cd1c87"
            }
          ]
        },
        {
          "id": "86de5a5b-8edb-40c2-9dc5-156d7d862afe",
          "name": "getIdentityPolicies",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityPolicies?Identity=Identity&PolicyNames.member.N=PolicyNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the requested sending authorization policies for the given identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a99cf00c-a47b-4b10-a634-15f75659067e"
            }
          ]
        },
        {
          "id": "325da60f-d3af-4320-b006-b99fb90b0906",
          "name": "getIdentityVerificationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityVerificationAttributes?Identities.member.N=Identities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a list of identities (email addresses and/or domains), returns the verification status and (for domain identities) the verification token for each identity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e083cc9b-13ef-4eb7-ad77-84580f84ddc7"
            }
          ]
        },
        {
          "id": "59912e1a-98c0-4098-a1dc-8016f473af19",
          "name": "listIdentities",
          "request": {
            "url": "http://example.com/api/?Action=ListIdentities?IdentityType=IdentityType&MaxItems=MaxItems&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list containing all of the identities (email addresses and domains) for your AWS account, regardless of verification status."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c3c32b7-4c96-4467-9ca0-f5eba367301a"
            }
          ]
        },
        {
          "id": "66e6bf17-e4d6-4cf2-a7e5-c96df7fde6ef",
          "name": "listIdentityPolicies",
          "request": {
            "url": "http://example.com/api/?Action=ListIdentityPolicies?Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of sending authorization policies that are attached to the given identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48a012ad-a128-489e-8458-48afe6670ef9"
            }
          ]
        },
        {
          "id": "155cb41d-9521-4cb2-921b-1a9d7ea275f6",
          "name": "putIdentityPolicy",
          "request": {
            "url": "http://example.com/api/?Action=PutIdentityPolicy?Identity=Identity&Policy=Policy&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or updates a sending authorization policy for the specified identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c35fee95-8472-41b2-85ea-8bcc4895be7b"
            }
          ]
        },
        {
          "id": "006914b9-a7ee-4923-81bc-a1378d9ab210",
          "name": "setIdentityDkimEnabled",
          "request": {
            "url": "http://example.com/api/?Action=SetIdentityDkimEnabled?DkimEnabled=DkimEnabled&Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables or disables Easy DKIM signing of email sent from an identity:If Easy DKIM\n            signing is enabled for a domain name identity (e."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56c07137-807e-4115-a619-130744238e52"
            }
          ]
        },
        {
          "id": "719cc090-4ad0-4672-afec-0868299753f5",
          "name": "setIdentityFeedbackForwardingEnabled",
          "request": {
            "url": "http://example.com/api/?Action=SetIdentityFeedbackForwardingEnabled?ForwardingEnabled=ForwardingEnabled&Identity=Identity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given an identity (an email address or a domain), enables or disables whether Amazon SES forwards bounce and complaint notifications as email."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "507361a2-5950-4d03-84ed-b10f8ccd8ef3"
            }
          ]
        },
        {
          "id": "b984fe3a-867e-402d-abeb-0cfe799ab969",
          "name": "setIdentityHeadersInNotificationsEnabled",
          "request": {
            "url": "http://example.com/api/?Action=SetIdentityHeadersInNotificationsEnabled?Enabled=Enabled&Identity=Identity&NotificationType=NotificationType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given an identity (an email address or a domain), sets whether Amazon SES includes \n            the original email headers in the Amazon Simple Notification Service (Amazon SNS) notifications \n            of a specified type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1bcee7f-40fe-4f5e-af03-f1dc56c847bb"
            }
          ]
        },
        {
          "id": "ed4e1e06-7754-498a-8a12-6a6b57fd7180",
          "name": "setIdentityMailFromDomain",
          "request": {
            "url": "http://example.com/api/?Action=SetIdentityMailFromDomain?BehaviorOnMXFailure=BehaviorOnMXFailure&Identity=Identity&MailFromDomain=MailFromDomain",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables or disables the custom MAIL FROM domain setup for a verified identity (an email address or a domain)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0fbc28c-c2e6-4d9e-8daf-e629350edd17"
            }
          ]
        }
      ]
    },
    {
      "name": "Verified Email Addresses",
      "item": [
        {
          "id": "93c37ac4-8550-4b1f-8873-c878c881f06e",
          "name": "deleteVerifiedEmailAddress",
          "request": {
            "url": "http://example.com/api/?Action=DeleteVerifiedEmailAddress?EmailAddress=EmailAddress",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified email address from the list of verified addresses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4133ae25-56de-4f05-86b7-841ab517685a"
            }
          ]
        },
        {
          "id": "32fdb82b-816a-4096-8d50-7d64ab907f89",
          "name": "listVerifiedEmailAddresses",
          "request": {
            "url": "http://example.com/api/?Action=ListVerifiedEmailAddresses?VerifiedEmailAddresses.member.N=VerifiedEmailAddresses.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list containing all of the email addresses that have been verified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c91bb4c-27a0-4204-86c8-8a37a1036a4a"
            }
          ]
        }
      ]
    },
    {
      "name": "Send Quota",
      "item": [
        {
          "id": "2733a022-64db-4a08-ab5a-46e1e6cd9db9",
          "name": "getSendQuota",
          "request": {
            "url": "http://example.com/api/?Action=GetSendQuota?Max24HourSend=Max24HourSend&MaxSendRate=MaxSendRate&SentLast24Hours=SentLast24Hours",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the user's current sending limits."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c817d2ad-db07-4a82-a430-5c81b5d8fd33"
            }
          ]
        }
      ]
    },
    {
      "name": "Send Statistics",
      "item": [
        {
          "id": "c32a815c-94da-4ea5-9e8a-3d16ab764a24",
          "name": "getSendStatistics",
          "request": {
            "url": "http://example.com/api/?Action=GetSendStatistics?SendDataPoints.member.N=SendDataPoints.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the user's sending statistics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6bd2297-dc9b-4df1-9fa7-4d790738f8d8"
            }
          ]
        }
      ]
    },
    {
      "name": "Bounce",
      "item": [
        {
          "id": "cacee4da-7f97-480a-9624-cc7a80dfaae7",
          "name": "sendBounce",
          "request": {
            "url": "http://example.com/api/?Action=SendBounce?BouncedRecipientInfoList.member.N=BouncedRecipientInfoList.member.N&BounceSender=BounceSender&BounceSenderArn=BounceSenderArn&Explanation=Explanation&MessageDsn=MessageDsn&OriginalMessageId=OriginalMessageId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Generates and sends a bounce message to the sender of an email you received through Amazon SES."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d7ff29f-69d8-4a15-8cc7-0ce7bbf746f6"
            }
          ]
        }
      ]
    },
    {
      "name": "Email",
      "item": [
        {
          "id": "6e651633-398b-4634-b5c4-d54c2e48bb9b",
          "name": "sendEmail",
          "request": {
            "url": "http://example.com/api/?Action=SendEmail?ConfigurationSetName=ConfigurationSetName&Destination=Destination&Message=Message&ReplyToAddresses.member.N=ReplyToAddresses.member.N&ReturnPath=ReturnPath&ReturnPathArn=ReturnPathArn&Source=Source&SourceArn=SourceArn&Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Composes an email message based on input data, and then immediately queues the message for sending."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a57ec4e5-bd03-45ed-8f48-37a18b718cc4"
            }
          ]
        },
        {
          "id": "5dcf13cf-5201-43f9-a9d6-f07f247d5243",
          "name": "sendRawEmail",
          "request": {
            "url": "http://example.com/api/?Action=SendRawEmail?ConfigurationSetName=ConfigurationSetName&Destinations.member.N=Destinations.member.N&FromArn=FromArn&RawMessage=RawMessage&ReturnPathArn=ReturnPathArn&Source=Source&SourceArn=SourceArn&Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sends an email message, with header and content specified by the client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8db471e-d3ab-4e38-a4e9-ffb0d89f0575"
            }
          ]
        }
      ]
    }
  ]
}