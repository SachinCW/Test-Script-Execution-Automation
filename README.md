# Test Script Execution Automation
The Jupyter notebook in this project has automatic script execution code. It connects to oracle databases 
using your credentials and fires queries that are supplied in its feeder file and produces a report that is 
emailed to the recipients of your choice. 
The report contains the test cases and color indicator to quickly let you know which test cases failed.
It also contains a pie chart with the number of test cases passed and failed.

You will need to provide your database hostname & DB SID. 
After the testing is completed, report is successfully generated and email sent, it also produces a voice and o/p terminal notification - it produces a beep and does announce through your laptop that testing is successfully completed. 
