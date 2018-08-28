swagger: "2.0"
x-collection-name: AWS Inspector
x-complete: 1
info:
  title: AWS Inspector API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RemoveAttributesFromFindings:
    get:
      summary: Remove Attributes From Findings
      description: |-
        Removes entire attributes (key and value pairs) from the findings that are specified
                 by the ARNs of the findings where an attribute with the specified key exists.
      operationId: removeAttributesFromFindings
      x-api-path-slug: actionremoveattributesfromfindings-get
      parameters:
      - in: query
        name: attributeKeys
        description: The array of attribute keys that you want to remove from specified         findings
        type: string
      - in: query
        name: findingArns
        description: The ARNs that specify the findings that you want to remove attributes
          from
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attributes From Findings
  /?Action=UnsubscribeFromEvent:
    get:
      summary: Unsubscribe From Event
      description: |-
        Disables the process of sending Amazon Simple Notification Service (SNS)
                 notifications about a specified event to a specified SNS topic.
      operationId: unsubscribeFromEvent
      x-api-path-slug: actionunsubscribefromevent-get
      parameters:
      - in: query
        name: event
        description: The event for which you want to stop receiving SNS notifications
        type: string
      - in: query
        name: resourceArn
        description: The ARN of the assessment template that is used during the event
          for which you want         to stop receiving SNS notifications
        type: string
      - in: query
        name: topicArn
        description: The ARN of the SNS topic to which SNS notifications are sent
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions