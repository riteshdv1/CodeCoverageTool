# CodeCoverageTool

<b>Introduction:</b>
<br/>
Test class execution and code coverage report generation in Salesforce has been a manual task where an individual had to execute the test classes and wait for their completion to generate the code coverage report.
<br/>
Further, comparison of previous coverage and current coverage for each class would require additional effort as it is a manual process until now.
<br/>
<br/>

<b>Solution:</b>
<br/>
This issue, could be addressed using automation so that manual efforts could be avoided and coverage reporting could be effortless and efficient.
<br/>
The code coverage reporting mechanism does this.
<br/>
<br/>
<b>Features of Code Coverage Reporting Mechanism:</b>
<br/>
•	Runs Test classes every day at a specifified time and generates report after the execution of test classes.
<br/>
•	Compares the previous and current coverage of each class.
<br/>
•	Provides details on previous and current total coverage.
<br/>
•	Provides details of failed test classes.
<br/>
•	Sends all these details through mail.
<br/>

<b>Brief Overview:</b>
<br/>
There are basically two jobs:
<br/>
<u>Code coverage starting job </u> : lists all the test classes and executes them at a specific time daily.
<br/>
<u>Code Coverage Reporting Job </u>: Runs after 2 hours of start of first job  (by this time all test classes would have executed), and then generates the report and sends it to the recipients.
<br/>
<br/>

<h1>Install From Here</h1> 
<br/>
  
Installation is still a Work in Progress

Sandbox : <a href="https://test.salesforce.com/packaging/installPackage.apexp?p0=04t7F000005145b" target="_blank">Click to install</a>
<br/>  
production : <a href="https://login.salesforce.com/packaging/installPackage.apexp?p0=04t7F000005145b" target="_blank">Click to install</a>

Password: Ritesh@123

Post Installation Step:
<br/>
<b>Step 1:</b> Create a remote site setting:
<br/>
Name: CodeCoverageSite
<br/>
Url: The base URL of org.
<br/>
Example: https://myorg.salesforce.com
<br/>
<br/>

<b>Step 2:</b> schedule the classes CodeCoverageStartingJob and CodeCoverageReportingJob with a interval of 2 hours between them.
<br/>
<br/>

<b>Additional Information:</b>
<br/>
To add the mail recipients, go to:
<b>custom setting >> CodeCoverageQueueSetting >> TestClassQueueId>>acctc__Email_Recipients__c</b>
and update the recipients.
<br/>
Please note, email addresses should be separated by comma.

 
  
