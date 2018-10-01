# CodeCoverageTool

Introduction:
Test class execution and code coverage report generation in Salesforce has been a manual task where an individual had to execute the test classes and wait for their completion to generate the code coverage report.
Further, comparison of previous coverage and current coverage for each class would require additional effort as it is a manual process until now.

Solution:
This issue, could be addressed using automation so that manual efforts could be avoided and coverage reporting could be effortless and efficient.
The code coverage reporting mechanism does this.

Features of Code Coverage Reporting Mechanism:
•	Runs Test classes every day at a specifified time and generates report after the execution of test classes.
•	Compares the previous and current coverage of each class.
•	Provides details on previous and current total coverage.
•	Provides details of failed test classes.
•	Sends all these details through mail.

Brief Overview:

There are basically two jobs:
Code coverage starting job: lists all the test classes and executes them at a specific time daily.
Code Coverage Reporting Job: Runs after 2 hours of start of first job  (by this time all test classes would have executed), and then generates the report and sends it to the recipients.



  <h1>Install From Here</h1> 
  <br/>
  
  Installation is still a Work in Progress
  
  <!--
  Sandbox : <a href="https://google.com" target="_blank">Click to install</a>
  <br/>  
  production : <a href="https://google.com" target="_blank">Click to install</a>
-->
 
  
