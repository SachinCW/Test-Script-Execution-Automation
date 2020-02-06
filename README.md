# Test Script Execution Automation

Overview:
The Jupyter notebook in this project has automatic script execution code. 
It helps automate testing of data completeness and data accuracy between different databases. It specifically tests the ETL ( Extraction, Transformation and Load ) process.

It connects to oracle databases using your credentials and fires queries that are supplied in its feeder file and produces a report that is 
emailed to the recipients of your choice. 
The report contains the test cases and color indicator to quickly let you know which test cases failed.
It also contains a pie chart with the number of test cases passed and failed.

After the testing is completed, report is successfully generated and email sent, it also produces a voice and o/p terminal notification - it produces a beep and does announce through your laptop that testing is successfully completed. 

How do you use this?
Prepare a feeder file ( example attached ) that has your test cases , scripts & expected count. The scripts for ETL testing should be written in such a way using Minus operations that you get the count of records. If data has moved accurately between databases in the ETL execution, then your script should produce a count of zero. If you get a non zero count, it means that the test case has failed and the data hasn't moved accurately as expected between databases.

You will need to provide your database hostname & DB SID. It gets username from windows system. For providing password to connect to database, you will need to enter the SID and the password in Windows Credential Manager. The keyring package then gets the password from Windows Credential Manager.
