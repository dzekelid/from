---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Transfer funds between bank accounts (also Deposit Cash/Cheques from
    Cash Held)
  version: 1.0.0
  description: Transfer funds between bank accounts (also deposit cash/cheques from
    cash held).
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/accounting/exports/batch/{id}/removepayment:
    put:
      summary: Remove an individual payment from batch export
      description: Remove an individual payment from batch export.
      operationId: AccountingExport_RemoveFromBatchByidBypaymentId
      x-api-path-slug: apiaccountingexportsbatchidremovepayment-put
      parameters:
      - in: path
        name: id
      - in: query
        name: paymentId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Individual
      - Payment
      - From
      - Batch
      - Export
  /api/auction/{id}/withdrawlots:
    post:
      summary: To withdraw a list of properties from the auction
      description: To withdraw a list of properties from the auction.
      operationId: Auction_WithdrawLotsByidBywithdrawLotsDataContract
      x-api-path-slug: apiauctionidwithdrawlots-post
      parameters:
      - in: path
        name: id
        description: The auction ID
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: withdrawLotsDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - To
      - Withdraw
      - List
      - Of
      - Properties
      - From
      - Auction
  /api/auction/removecontact:
    post:
      summary: Remove an existing auction contact from the auction role
      description: Remove an existing auction contact from the auction role.
      operationId: Auction_RemoveAuctionContactByremoveContactDataContract
      x-api-path-slug: apiauctionremovecontact-post
      parameters:
      - in: body
        name: removeContactDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Existing
      - Auction
      - Contact
      - From
      - Auction
      - Role
  /api/branding/{id}/detachdocument:
    put:
      summary: Detaches a document from a brand.
      description: Detaches a document from a brand..
      operationId: Branding_DetachDocumentByidBydocumentId
      x-api-path-slug: apibrandingiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The documentId
      - in: path
        name: id
        description: The BrandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Brand
  /api/cache/List/{listKey}/Item:
    delete:
      summary: Removes a given item from the list.
      description: Removes a given item from the list..
      operationId: Cache_RemoveItemFromListByitemToRemoveBylistKey
      x-api-path-slug: apicachelistlistkeyitem-delete
      parameters:
      - in: body
        name: itemToRemove
        description: The item to remove
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Given
      - Item
      - From
      - List
  /api/cache/List/{listKey}/Pop:
    get:
      summary: Pops an items from the list head.
      description: Pops an items from the list head..
      operationId: Cache_PopFromListHeadBylistKey
      x-api-path-slug: apicachelistlistkeypop-get
      parameters:
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Pops
      - Items
      - From
      - List
      - Head
  /api/dashboard/{id}/removewidgets:
    put:
      summary: Remove widgets from a dashboard
      description: Remove widgets from a dashboard.
      operationId: Dashboard_RemoveWidgetsFromDashboardByid
      x-api-path-slug: apidashboardidremovewidgets-put
      parameters:
      - in: path
        name: id
        description: Dashboard Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Widgets
      - From
      - Dashboard
  /api/todo/canceltodo:
    put:
      summary: Cancel a to-do list from the tile overview of to-dos
      description: Cancel a to-do list from the tile overview of to-dos.
      operationId: DefaultToDo_CancelTodoBycancelTodoCommandData
      x-api-path-slug: apitodocanceltodo-put
      parameters:
      - in: body
        name: cancelTodoCommandData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - To-do
      - List
      - From
      - Tile
      - Overview
      - Of
      - To-dos
  /api/todo/canceltasks:
    put:
      summary: Cancel a single or multiple tasks from a to-do bucket
      description: Cancel a single or multiple tasks from a to-do bucket.
      operationId: DefaultToDo_CancelTasksBycancelTasksCommandData
      x-api-path-slug: apitodocanceltasks-put
      parameters:
      - in: body
        name: cancelTasksCommandData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Single
      - Multiple
      - Tasks
      - From
      - To-do
      - Bucket
  /api/document/setprivacy:
    put:
      summary: Sets the document privacy for an existing document.  This is used to
        change a document from being publicly accessible to being private, and vice
        versa.
      description: Sets the document privacy for an existing document.  this is used
        to change a document from being publicly accessible to being private, and
        vice versa..
      operationId: Document_SetDocumentPrivacyBysetDocumentPrivacyCommand
      x-api-path-slug: apidocumentsetprivacy-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setDocumentPrivacyCommand
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Document
      - Privacyan
      - Existing
      - Document
      - ""
      - ""
      - This
      - Is
      - Used
      - To
      - Change
      - Document
      - From
      - Being
      - Publicly
      - Accessible
      - To
      - Being
      - Private
      - ""
      - Vice
      - Versa
  /api/documentgeneration/deletesackcontent/{sackReference}/{envelopereference}:
    get:
      summary: "deletes an envelope from the the content of a sack \r\nDeprecated
        in favour of the DELETE verb"
      description: "Deletes an envelope from the the content of a sack \r\ndeprecated
        in favour of the delete verb."
      operationId: DocumentGeneration_DeleteSackContentDeprecatedBysackReferenceByenvelopereference
      x-api-path-slug: apidocumentgenerationdeletesackcontentsackreferenceenvelopereference-get
      parameters:
      - in: path
        name: envelopereference
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: sackReference
      responses:
        200:
          description: OK
      tags:
      - Deletes
      - Envelope
      - From
      - The
      - Content
      - Of
      - Sack
      - Deprecated
      - In
      - Favour
      - Of
      - DELETE
      - Verb
  /api/documentgeneration/sackcontent/{sackReference}/{envelopereference}:
    delete:
      summary: deletes an envelope from the the content of a sack
      description: Deletes an envelope from the the content of a sack.
      operationId: DocumentGeneration_DeleteSackContentBysackReferenceByenvelopereference
      x-api-path-slug: apidocumentgenerationsackcontentsackreferenceenvelopereference-delete
      parameters:
      - in: path
        name: envelopereference
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: sackReference
      responses:
        200:
          description: OK
      tags:
      - Deletes
      - Envelope
      - From
      - The
      - Content
      - Of
      - Sack
  /api/documentgeneration/envelopecontent/{sackReference}/{envelopereference}/{documentreference}:
    delete:
      summary: deletes an document from an envelope
      description: Deletes an document from an envelope.
      operationId: DocumentGeneration_DeleteEnvelopeContentBysackReferenceByenvelopereferenceBydocumentreference
      x-api-path-slug: apidocumentgenerationenvelopecontentsackreferenceenvelopereferencedocumentreference-delete
      parameters:
      - in: path
        name: documentreference
      - in: path
        name: envelopereference
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: sackReference
      responses:
        200:
          description: OK
      tags:
      - Deletes
      - Document
      - From
      - Envelope
  /api/documentgeneration/sack/{sackReference}:
    delete:
      summary: deletes an envelope from the the content of a sack
      description: Deletes an envelope from the the content of a sack.
      operationId: DocumentGeneration_DeleteSackBysackReference
      x-api-path-slug: apidocumentgenerationsacksackreference-delete
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: sackReference
      responses:
        200:
          description: OK
      tags:
      - Deletes
      - Envelope
      - From
      - The
      - Content
      - Of
      - Sack
  /api/documentgeneration/printsackcontent/{sackReference}/{envelopereference}:
    get:
      summary: Prints an envelope from a sack
      description: Prints an envelope from a sack.
      operationId: DocumentGeneration_PrintSackContentBysackReferenceByenvelopereference
      x-api-path-slug: apidocumentgenerationprintsackcontentsackreferenceenvelopereference-get
      parameters:
      - in: path
        name: envelopereference
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: sackReference
      responses:
        200:
          description: OK
      tags:
      - Prints
      - Envelope
      - From
      - Sack
  /api/documentgeneration/deleteprintenvelopes:
    delete:
      summary: Delete Print Envelopes from the print bags
      description: Delete print envelopes from the print bags.
      operationId: DocumentGeneration_DeletePrintEnvelopesByprintBagDataContract
      x-api-path-slug: apidocumentgenerationdeleteprintenvelopes-delete
      parameters:
      - in: body
        name: printBagDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Print
      - Envelopes
      - From
      - Print
      - Bags
  /api/group/{id}/deletegroupmember:
    delete:
      summary: Delete a contact from a group
      description: Delete a contact from a group.
      operationId: Group_DeleteGroupMemberByidBydeleteCommand
      x-api-path-slug: apigroupiddeletegroupmember-delete
      parameters:
      - in: body
        name: deleteCommand
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Contact
      - From
      - Group
  /api/group/{id}/deletesearch/{searchingRoleId}:
    delete:
      summary: Deletes Search Criteria from a Group
      description: Deletes search criteria from a group.
      operationId: Group_DeleteSearchByidBysearchingRoleId
      x-api-path-slug: apigroupiddeletesearchsearchingroleid-delete
      parameters:
      - in: path
        name: id
        description: The id of the group
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: searchingRoleId
        description: The id of the searching role to delete
      responses:
        200:
          description: OK
      tags:
      - S
      - Search
      - Criteria
      - From
      - Group
  /api/group/{id}/detachdocument:
    put:
      summary: Detaches a document from a group
      description: Detaches a document from a group.
      operationId: Group_DetachDocumentByidBydocumentId
      x-api-path-slug: apigroupiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to detach
      - in: path
        name: id
        description: The id of the group to detach the document from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Group
  /api/group/{id}/getpropertyroleidsalreadysent:
    get:
      summary: returns a list of the property role ids that should be excluded from
        mailouts to this role id because the have been sent before
      description: Returns a list of the property role ids that should be excluded
        from mailouts to this role id because the have been sent before.
      operationId: Group_GetPropertyMarketingRoleIdsSentByidBywithinDaysByresendPriceChangedProperties
      x-api-path-slug: apigroupidgetpropertyroleidsalreadysent-get
      parameters:
      - in: path
        name: id
        description: The id of the group
      - in: query
        name: resendPriceChangedProperties
        description: include the properties that have had to a price change or withdrawn
          event since it was last sent to them
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: withinDays
        description: number of days since the last time it was sent, send 0 for all
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Property
      - Role
      - Ids
      - That
      - Should
      - Be
      - Excluded
      - From
      - Mailouts
      - To
      - This
      - Role
      - Id
      - Because
      - Have
      - Been
      - Sent
      - Before
  /api/identity/Remove:
    put:
      summary: Removes an identity (E.g. Facebook Identity, Twitter identity etc.)
        from a person
      description: Removes an identity (e.g. facebook identity, twitter identity etc.)
        from a person.
      operationId: Identity_RemoveIdentityFromPersonBypersonIdByidentityId
      x-api-path-slug: apiidentityremove-put
      parameters:
      - in: query
        name: identityId
      - in: query
        name: personId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Identity
      - (E
      - G
      - ""
      - Facebook
      - Identity
      - ""
      - Twitter
      - Identity
      - Etc
      - )
      - From
      - Person
  /api/invoice/{id}/removefee:
    put:
      summary: Remove fee from existing invoice
      description: Remove fee from existing invoice.
      operationId: Invoice_RemoveLinkedFeeByidByattachedFeeId
      x-api-path-slug: apiinvoiceidremovefee-put
      parameters:
      - in: query
        name: attachedFeeId
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Fee
      - From
      - Existing
      - Invoice
  /api/progression/lettings/detatchdocumentfromlandlord:
    post:
      summary: Detatch a document from a landlord.
      description: Detatch a document from a landlord..
      operationId: LettingsProgression_DetatchDocumentFromLandlordBylandlordInfoIdBydocumentId
      x-api-path-slug: apiprogressionlettingsdetatchdocumentfromlandlord-post
      parameters:
      - in: query
        name: documentId
        description: The tenant Id
      - in: query
        name: landlordInfoId
        description: The tenant Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detatch
      - Document
      - From
      - Landlord
  /api/progression/lettings/detatchdocumentfromtenant:
    post:
      summary: Detatch a document from a landlord.
      description: Detatch a document from a landlord..
      operationId: LettingsProgression_DetatchDocumentFromTenantBytenantInfoIdBydocumentId
      x-api-path-slug: apiprogressionlettingsdetatchdocumentfromtenant-post
      parameters:
      - in: query
        name: documentId
        description: The tenant Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tenantInfoId
        description: The tenant Id
      responses:
        200:
          description: OK
      tags:
      - Detatch
      - Document
      - From
      - Landlord
  /api/progression/lettings/detatchdocumentfromguarantor:
    post:
      summary: Detatch a document from a landlord.
      description: Detatch a document from a landlord..
      operationId: LettingsProgression_DetatchDocumentFromGuarantorByguarantorIdBydocumentIdBypersonId
      x-api-path-slug: apiprogressionlettingsdetatchdocumentfromguarantor-post
      parameters:
      - in: query
        name: documentId
        description: The tenant Id
      - in: query
        name: guarantorId
        description: The tenant Id
      - in: query
        name: personId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detatch
      - Document
      - From
      - Landlord
  /api/progression/lettings/detatchdocumentfromreference:
    post:
      summary: Detatch a document from a reference.
      description: Detatch a document from a reference..
      operationId: LettingsProgression_DetatchDocumentFromReferenceByreferenceIdBydocumentId
      x-api-path-slug: apiprogressionlettingsdetatchdocumentfromreference-post
      parameters:
      - in: query
        name: documentId
        description: The tenant Id
      - in: query
        name: referenceId
        description: The tenant Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detatch
      - Document
      - From
      - Reference
  /api/progression/lettings/{roleId}/removetenantcharge:
    delete:
      summary: Remove charges from a tenant role
      description: Remove charges from a tenant role.
      operationId: LettingsProgression_RemoveTenantChargesByroleIdBychargeIds
      x-api-path-slug: apiprogressionlettingsroleidremovetenantcharge-delete
      parameters:
      - in: query
        name: chargeIds
        description: The ids of the charges to remove
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
        description: The tenant role id
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Charges
      - From
      - Tenant
      - Role
  /api/list/property/csv:
    post:
      summary: Generates a csv file from selected property list items
      description: Generates a csv file from selected property list items.
      operationId: List_GeneratePropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertycsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Property
      - List
      - Items
  /api/list/lettingproperty/csv:
    post:
      summary: Generates a csv file from selected letting property list items
      description: Generates a csv file from selected letting property list items.
      operationId: List_GenerateLettingPropertyCsvBycommandDataContract
      x-api-path-slug: apilistlettingpropertycsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Letting
      - Property
      - List
      - Items
  /api/list/propertypipeline/csv:
    post:
      summary: Generates a csv file from selected property list items
      description: Generates a csv file from selected property list items.
      operationId: List_GeneratePipelinePropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertypipelinecsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Property
      - List
      - Items
  /api/list/events/csv:
    post:
      summary: Generates a csv file from selected event list items
      description: Generates a csv file from selected event list items.
      operationId: List_GenerateEventCsvBycommandDataContract
      x-api-path-slug: apilisteventscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Event
      - List
      - Items
  /api/list/groups/csv:
    post:
      summary: Generates a csv file from selected group list items
      description: Generates a csv file from selected group list items.
      operationId: List_GenerateGroupCsvBycommandDataContract
      x-api-path-slug: apilistgroupscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - List
      - Items
  /api/list/groupinterests/csv:
    post:
      summary: Generates a csv file from selected group interest list items
      description: Generates a csv file from selected group interest list items.
      operationId: List_GenerateGroupInterestCsvBycommandDataContract
      x-api-path-slug: apilistgroupinterestscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - Interest
      - List
      - Items
  /api/list/activesearches/csv:
    post:
      summary: Generates a csv file from selected group list items
      description: Generates a csv file from selected group list items.
      operationId: List_GenerateActiveSearchCsvBycommandDataContract
      x-api-path-slug: apilistactivesearchescsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - List
      - Items
  /api/list/groupmatches/csv:
    post:
      summary: Generates a csv file from group matches by property role id
      description: Generates a csv file from group matches by property role id.
      operationId: List_GenerateGroupMatchesCsvBycommandDataContract
      x-api-path-slug: apilistgroupmatchescsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Group
      - Matches
      - By
      - Property
      - Role
      - Id
  /api/list/propertyfinancial/csv:
    post:
      summary: Generates a csv file from selected group list items
      description: Generates a csv file from selected group list items.
      operationId: List_GenerateFinancialPropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertyfinancialcsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - List
      - Items
  /api/list/propertynewbusiness/csv:
    post:
      summary: Generates a csv file from selected property list items
      description: Generates a csv file from selected property list items.
      operationId: List_GenerateNewBusinessPropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertynewbusinesscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Property
      - List
      - Items
  /api/milestone/{id}/detachdocument:
    put:
      summary: Detaches a document from a milestone
      description: Detaches a document from a milestone.
      operationId: Milestone_DetachDocumentByidBydocumentId
      x-api-path-slug: apimilestoneiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to detach
      - in: path
        name: id
        description: The id of the milestone to detach the document from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Milestone
  /api/negotiator/my/properties/favourite/remove/{propertyId}:
    delete:
      summary: Remove a property from a Negotiators favourite list.
      description: Remove a property from a negotiators favourite list..
      operationId: Negotiator_RemoveFavouritePropertyBypropertyIdByroleId
      x-api-path-slug: apinegotiatormypropertiesfavouriteremovepropertyid-delete
      parameters:
      - in: path
        name: propertyId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Property
      - From
      - Negotiators
      - Favourite
      - List
  /api/negotiator/my/groups/favourite/remove/{groupId}:
    delete:
      summary: Remove a group from a Negotiators favourite list.
      description: Remove a group from a negotiators favourite list..
      operationId: Negotiator_RemoveFavouriteGroupBygroupId
      x-api-path-slug: apinegotiatormygroupsfavouriteremovegroupid-delete
      parameters:
      - in: path
        name: groupId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Group
      - From
      - Negotiators
      - Favourite
      - List
  /api/people/{id}/removecontactitem/{contactItemid}:
    put:
      summary: Remove a ContactItem from a Person
      description: Remove a contactitem from a person.
      operationId: People_RemoveContactItemByidBycontactItemid
      x-api-path-slug: apipeopleidremovecontactitemcontactitemid-put
      parameters:
      - in: path
        name: contactItemid
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - ContactItem
      - From
      - Person
  /api/people/{id}/removeaddress/{addressId}:
    put:
      summary: Remove an Address from a Person
      description: Remove an address from a person.
      operationId: People_RemoveAddressByidByaddressId
      x-api-path-slug: apipeopleidremoveaddressaddressid-put
      parameters:
      - in: path
        name: addressId
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Ress
      - From
      - Person
  /api/poi/search/radius:
    post:
      summary: Search for POI's in a radius from a point
      description: Search for poi's in a radius from a point.
      operationId: Poi_GeoRadiusSearchByquery
      x-api-path-slug: apipoisearchradius-post
      parameters:
      - in: body
        name: query
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - SearchPOIs
      - In
      - Radius
      - From
      - Point
  /api/progression/removecontact:
    post:
      summary: Remove an existing progression contact from the progression role
      description: Remove an existing progression contact from the progression role.
      operationId: Progression_RemoveProgressionContactByremoveContactDataContract
      x-api-path-slug: apiprogressionremovecontact-post
      parameters:
      - in: body
        name: removeContactDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Existing
      - Progression
      - Contact
      - From
      - Progression
      - Role
  /api/property/{id}/detachdocument:
    put:
      summary: Detaches a document from a property
      description: Detaches a document from a property.
      operationId: Property_DetachDocumentByidBydocumentId
      x-api-path-slug: apipropertyiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to detach
      - in: path
        name: id
        description: The id of the property description to detach the document from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Property
  /api/property/{id}/keys/remove:
    delete:
      summary: Remove keys from a property
      description: Remove keys from a property.
      operationId: Property_RemoveKeysByidBykeyIds
      x-api-path-slug: apipropertyidkeysremove-delete
      parameters:
      - in: path
        name: id
        description: The property id
      - in: query
        name: keyIds
        description: The ids of the keys to remove
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Keys
      - From
      - Property
  /api/property/{id}/alarms/remove:
    delete:
      summary: Remove alarm codes from a property
      description: Remove alarm codes from a property.
      operationId: Property_RemoveAlarmsByidByalarmIds
      x-api-path-slug: apipropertyidalarmsremove-delete
      parameters:
      - in: query
        name: alarmIds
        description: The ids of the alarm codes to remove
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Alarm
      - Codes
      - From
      - Property
  /api/property/{id}/specialarrangements/remove:
    delete:
      summary: Remove special arrangements from a property
      description: Remove special arrangements from a property.
      operationId: Property_RemoveSpecialArrangementsByidByarrangementIds
      x-api-path-slug: apipropertyidspecialarrangementsremove-delete
      parameters:
      - in: query
        name: arrangementIds
        description: The ids of the special arrangements to remove
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Special
      - Arrangements
      - From
      - Property
  /api/property/{id}/certificate/remove:
    delete:
      summary: Remove certificate from a property
      description: Remove certificate from a property.
      operationId: Property_RemoveCertificateByidBycertificateId
      x-api-path-slug: apipropertyidcertificateremove-delete
      parameters:
      - in: query
        name: certificateId
        description: The ids of the certificate to remove
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Certificate
      - From
      - Property
  /api/property/{id}/tenantroles:
    get:
      summary: Get a list of all current and ended tenant roles from a property id.
      description: Get a list of all current and ended tenant roles from a property
        id..
      operationId: Property_TenantRolesByPropertyIdByid
      x-api-path-slug: apipropertyidtenantroles-get
      parameters:
      - in: path
        name: id
        description: The Id of the property
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - Current
      - Ended
      - Tenant
      - Roles
      - From
      - Property
      - Id
  /api/receipt/fundsshortfall:
    post:
      summary: Records funds from office account into client account and then to client
        if necessary.
      description: Records funds from office account into client account and then
        to client if necessary..
      operationId: Receipt_ReceiptFundsShortfallBydataContract
      x-api-path-slug: apireceiptfundsshortfall-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Records
      - Funds
      - From
      - Office
      - Account
      - Into
      - Client
      - Account
      - Then
      - To
      - Client
      - If
      - Necessary
  /api/region/favourites/{favouriteRegionId}:
    delete:
      summary: Remove a region from your favourites
      description: Remove a region from your favourites.
      operationId: Region_RemoveFavouriteByfavouriteRegionId
      x-api-path-slug: apiregionfavouritesfavouriteregionid-delete
      parameters:
      - in: path
        name: favouriteRegionId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Region
      - From
      - Your
      - Favourites
  /api/role/{id}/detachdescription:
    put:
      summary: Detaches a description from a role
      description: Detaches a description from a role.
      operationId: Role_DetachDescriptionByidBydescriptionId
      x-api-path-slug: apiroleiddetachdescription-put
      parameters:
      - in: query
        name: descriptionId
        description: The id of the description to detach
      - in: path
        name: id
        description: The id of the role to detach the description from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Description
      - From
      - Role
  /api/role/{id}/detachdocument:
    put:
      summary: Detaches a document from a role
      description: Detaches a document from a role.
      operationId: Role_DetachDocumentByidBydocumentId
      x-api-path-slug: apiroleiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to detach
      - in: path
        name: id
        description: The id of the role to detach the document from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Role
  /api/role/{id}/removefee:
    put:
      summary: Remove a fee from a given PropertyMarketingRole.
      description: Remove a fee from a given propertymarketingrole..
      operationId: Role_RemoveFeeByidByfeeId
      x-api-path-slug: apiroleidremovefee-put
      parameters:
      - in: query
        name: feeId
        description: The Id of the fee to remove
      - in: path
        name: id
        description: the id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Fee
      - From
      - Given
      - PropertyMarketingRole
  /api/role/{id}/removeholdingdeposit:
    post:
      summary: Remove holding deposit from role
      description: Remove holding deposit from role.
      operationId: Role_RemoveHoldingDepositByidByrelatedRoleId
      x-api-path-slug: apiroleidremoveholdingdeposit-post
      parameters:
      - in: path
        name: id
      - in: query
        name: relatedRoleId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Holding
      - Deposit
      - From
      - Role
  /api/roomdescription/{id}/detachdocumentfromroom:
    put:
      summary: Detaches a document from a room description room.
      description: Detaches a document from a room description room..
      operationId: RoomDescription_DetachDocumentFromRoomByidBydocumentIdByroomId
      x-api-path-slug: apiroomdescriptioniddetachdocumentfromroom-put
      parameters:
      - in: query
        name: documentId
        description: The document Id
      - in: path
        name: id
        description: The room description Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roomId
        description: The room Id
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Room
      - Description
      - Room
  /api/role/sales/{id}/getepc:
    get:
      summary: Gets EPC from the supplied propertyRoleId
      description: Gets epc from the supplied propertyroleid.
      operationId: SalesRole_GetEPCByid
      x-api-path-slug: apirolesalesidgetepc-get
      parameters:
      - in: path
        name: id
        description: The role id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - EPC
      - From
      - Supplied
      - PropertyRoleId
  /api/sync/cronofycallback/{negotiatorId}/{uniqueIdentifier}:
    post:
      summary: Forces a call to get updates from Cronofy for the rezi calendar
      description: Forces a call to get updates from cronofy for the rezi calendar.
      operationId: Sync_CronofyCallbackBynegotiatorIdByuniqueIdentifierBycalendarSyncResyncDataContract
      x-api-path-slug: apisynccronofycallbacknegotiatoriduniqueidentifier-post
      parameters:
      - in: body
        name: calendarSyncResyncDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: negotiatorId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: uniqueIdentifier
      responses:
        200:
          description: OK
      tags:
      - Forces
      - Call
      - To
      - Get
      - Updates
      - From
      - Cronofythe
      - Rezi
      - Calendar
  /api/sync/deletecalendar:
    delete:
      summary: Forces a call to get updates from Cronofy for the rezi calendar
      description: Forces a call to get updates from cronofy for the rezi calendar.
      operationId: Sync_DeleteCalendar
      x-api-path-slug: apisyncdeletecalendar-delete
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Forces
      - Call
      - To
      - Get
      - Updates
      - From
      - Cronofythe
      - Rezi
      - Calendar
  /api/teams/{id}/members/remove:
    post:
      summary: Remove a member from a team
      description: Remove a member from a team.
      operationId: Teams_RemoveMemberByidByremoveTeamMemberCommand
      x-api-path-slug: apiteamsidmembersremove-post
      parameters:
      - in: path
        name: id
        description: Team Id
      - in: body
        name: removeTeamMemberCommand
        description: Details of team members
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Member
      - From
      - Team
  /api/tenancy/{id}/detachdocument:
    put:
      summary: Detaches a document from a tenancy role
      description: Detaches a document from a tenancy role.
      operationId: Tenancy_DetachDocumentByidBydocumentId
      x-api-path-slug: apitenancyiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to detach
      - in: path
        name: id
        description: The id of the role to detach the document from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Tenancy
      - Role
  /api/tenancy/{id}/removeadditionalservice/{additionalServiceId}:
    post:
      summary: Remove additional service from tenancy
      description: Remove additional service from tenancy.
      operationId: Tenancy_DeleteAdditionalServiceByidByadditionalServiceId
      x-api-path-slug: apitenancyidremoveadditionalserviceadditionalserviceid-post
      parameters:
      - in: path
        name: additionalServiceId
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Additional
      - Service
      - From
      - Tenancy
  /api/transfer/interaccount:
    post:
      summary: Transfer funds between bank accounts (also Deposit Cash/Cheques from
        Cash Held)
      description: Transfer funds between bank accounts (also deposit cash/cheques
        from cash held).
      operationId: Transfer_ProcessIatByiatDataContract
      x-api-path-slug: apitransferinteraccount-post
      parameters:
      - in: body
        name: iatDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Transfer
      - Funds
      - Between
      - Bank
      - Accounts
      - (also
      - Deposit
      - Cash
      - Cheques
      - From
      - Cash
      - Held)
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---