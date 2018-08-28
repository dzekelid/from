---
swagger: "2.0"
x-collection-name: PayRun
x-complete: 0
info:
  title: Pay Run.IO Gets the specified reporting instruction from the employer
  description: Returns the specified pay instruction from employee
  version: 17.18.6.206
host: api.test.payrun.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Employer/{EmployerId}/Employee/{EmployeeId}:
    get:
      summary: Get employee from employer
      description: Gets the specified employee from employer by employee code.
      operationId: GetEmployeeFromEmployer
      x-api-path-slug: employeremployeridemployeeemployeeid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employee
      - From
      - Employer
  /Employer/{EmployerId}/Employee/{EmployeeId}/Commentary/{CommentaryId}:
    get:
      summary: Get commentary from employee
      description: Gets the specified commentary report from the employee
      operationId: GetCommentaryFromEmployee
      x-api-path-slug: employeremployeridemployeeemployeeidcommentarycommentaryid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: CommentaryId
        description: The commentary unique identifier
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Commentary
      - From
      - Employee
  /Employer/{EmployerId}/Employee/{EmployeeId}/PayInstruction/{PayInstructionId}:
    get:
      summary: Gets the specified pay instruction from the employee
      description: Returns the specified pay instruction from employee
      operationId: GetPayInstructionFromEmployee
      x-api-path-slug: employeremployeridemployeeemployeeidpayinstructionpayinstructionid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayInstructionId
        description: The pay instruction unique identifier
      responses:
        200:
          description: OK
      tags:
      - Specified
      - Pay
      - Instruction
      - From
      - Employee
  /Employer/{EmployerId}/Employee/{EmployeeId}/PayInstructions:
    get:
      summary: Gets the pay instructions from the specified employee
      description: Get links to all pay instructions for the specified employee
      operationId: GetPayInstructionsFromEmployee
      x-api-path-slug: employeremployeridemployeeemployeeidpayinstructions-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Instructions
      - From
      - Specified
      - Employee
  /Employer/{EmployerId}/Employee/{EmployeeId}/PayLine/{PayLineId}:
    get:
      summary: Gets the specified pay line from the employee
      description: Returns the specified pay line from employee
      operationId: GetPayLineFromEmployee
      x-api-path-slug: employeremployeridemployeeemployeeidpaylinepaylineid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayLineId
        description: The pay line unique identifier
      responses:
        200:
          description: OK
      tags:
      - Specified
      - Pay
      - Line
      - From
      - Employee
  /Employer/{EmployerId}/Employee/{EmployeeId}/PayLines:
    get:
      summary: Gets the pay lines from the specified employee
      description: Get links to all pay lines for the specified employee
      operationId: GetPayLinesFromEmployee
      x-api-path-slug: employeremployeridemployeeemployeeidpaylines-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Lines
      - From
      - Specified
      - Employee
  /Employer/{EmployerId}/Employee/{EmployeeId}/PayRuns:
    get:
      summary: Gets the pay runs from the employee
      description: Get links to all pay runs for the specified employee.
      operationId: GetPayRunsFromEmployee
      x-api-path-slug: employeremployeridemployeeemployeeidpayruns-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Runs
      - From
      - Employee
  /Employer/{EmployerId}/Employees:
    get:
      summary: Get employees from employer.
      description: Get links to all employees for the specified employer.
      operationId: GetEmployeesFromEmployer
      x-api-path-slug: employeremployeridemployees-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employees
      - From
      - Employer
  /Employer/{EmployerId}/Employees/{EffectiveDate}:
    get:
      summary: Get employees from employer at a given effective date.
      description: Get links to all employees for the employer on specified effective
        date.
      operationId: GetEmployeesByEffectiveDate
      x-api-path-slug: employeremployeridemployeeseffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employees
      - From
      - Employer
      - At
      - Given
      - Effective
      - Date
  /Employer/{EmployerId}/PayCode/{PayCodeId}:
    get:
      summary: Gets the specified pay code from the employer
      description: Returns the specified pay code from the employer
      operationId: GetPayCodeFromEmployer
      x-api-path-slug: employeremployeridpaycodepaycodeid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayCodeId
        description: The pay code unique identifier
      responses:
        200:
          description: OK
      tags:
      - Specified
      - Pay
      - Code
      - From
      - Employer
  /Employer/{EmployerId}/PayCodes:
    get:
      summary: Gets the pay codes from the employer
      description: Get links to all the pay codes for the specified employer
      operationId: GetPayCodesFromEmployer
      x-api-path-slug: employeremployeridpaycodes-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Codes
      - From
      - Employer
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}:
    get:
      summary: Gets the specified pay schedule from the employer
      description: Returns the specified pay schedule object from employer
      operationId: GetPayScheduleFromEmployer
      x-api-path-slug: employeremployeridpayschedulepayscheduleid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Specified
      - Pay
      - Schedule
      - From
      - Employer
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/Employees:
    get:
      summary: Get employees from a pay schedule.
      description: Gets links to all employees included in the specified pay schedule.
      operationId: GetEmployeesFromPaySchedule
      x-api-path-slug: employeremployeridpayschedulepayscheduleidemployees-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employees
      - From
      - Pay
      - Schedule
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}:
    get:
      summary: Gets the pay run from the pay schedule
      description: Returns the pay run from the pay schedule
      operationId: GetPayRunFromPaySchedule
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - From
      - Pay
      - Schedule
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}/Employees:
    get:
      summary: Get employees from the pay run
      description: Gets links to all employees included in the specified pay run.
      operationId: GetEmployeesFromPayRun
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidemployees-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employees
      - From
      - Pay
      - Run
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}/ReportLines:
    get:
      summary: Gets the report lines from the specified pay run
      description: Returns all report lines associated with the specified pay run
      operationId: GetReportLinesFromPayRun
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidreportlines-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Report
      - Lines
      - From
      - Specified
      - Pay
      - Run
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRuns:
    get:
      summary: Gets the pay runs from the pay schedule
      description: Get links to all pay runs for the specified pay schedule
      operationId: GetPayRunsFromPaySchedule
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayruns-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Runs
      - From
      - Pay
      - Schedule
  /Employer/{EmployerId}/PaySchedules:
    get:
      summary: Gets the pay schedule from the specified employer
      description: Get links to all pay schedules for the specified employer
      operationId: GetPaySchedulesFromEmployer
      x-api-path-slug: employeremployeridpayschedules-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Schedule
      - From
      - Specified
      - Employer
  /Employer/{EmployerId}/Pension/{PensionId}:
    get:
      summary: Get pension from employer
      description: Gets the specified pension from employer by pension code.
      operationId: GetPensionFromEmployer
      x-api-path-slug: employeremployeridpensionpensionid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PensionId
        description: The pensions unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pension
      - From
      - Employer
  /Employer/{EmployerId}/Pensions:
    get:
      summary: Get pensions from employer.
      description: Get links to all pensions for the specified employer.
      operationId: GetPensionsFromEmployer
      x-api-path-slug: employeremployeridpensions-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pensions
      - From
      - Employer
  /Employer/{EmployerId}/Pensions/{EffectiveDate}:
    get:
      summary: Get pensions from employer at a given effective date.
      description: Get links to all pensions for the employer on specified effective
        date.
      operationId: GetPensionsByEffectiveDate
      x-api-path-slug: employeremployeridpensionseffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pensions
      - From
      - Employer
      - At
      - Given
      - Effective
      - Date
  /Employer/{EmployerId}/ReportLine/{ReportLineId}:
    get:
      summary: Gets the specified report line from the employer
      description: Returns the specified pay line from employee
      operationId: GetReportLineFromEmployer
      x-api-path-slug: employeremployeridreportlinereportlineid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: ReportLineId
        description: The report line unique identifier
      responses:
        200:
          description: OK
      tags:
      - Specified
      - Report
      - Line
      - From
      - Employer
  /Employer/{EmployerId}/ReportLines:
    get:
      summary: Gets the report lines from the specified employer
      description: Get links to all report lines for the specified employee
      operationId: GetReportLinesFromEmployer
      x-api-path-slug: employeremployeridreportlines-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Report
      - Lines
      - From
      - Specified
      - Employer
  /Employer/{EmployerId}/ReportingInstruction/{ReportingInstructionId}:
    get:
      summary: Gets the specified reporting instruction from the employer
      description: Returns the specified pay instruction from employee
      operationId: GetReportingInstructionFromEmployer
      x-api-path-slug: employeremployeridreportinginstructionreportinginstructionid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: ReportingInstructionId
        description: The reporting instruction unique identifier
      responses:
        200:
          description: OK
      tags:
      - Specified
      - Reporting
      - Instruction
      - From
      - Employer
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