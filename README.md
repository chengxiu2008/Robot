# Robot
This is for robot framework staffs.
# Robot framework 
* Robot installation path - > C:\Python27\Lib\site-packages\robot
## Source Code Structure
  * rebot.py
    * Module implementing the command line entry point for post-processing
    * **python rebot.py output.xml**  (generate the log.html and report.html)
    * output.xml: \<statistics> ... \</statistics> is not necessary for generating the log.html, script rebot.py will do the calculation based on the input output.xml result.
  * run.py
    * Module implementing the command line entry point for executing tests
    * Go into the case top-level folder and call the run.py
       1. Run **all case** in test data Common_testcase.txt
          * run.py Common_Cases\Common_testcase.txt
       2. Run **one case Pre** in test_data_1.txt
          * run.py -t Pre Common_Cases\Common_testcase.txt
       3. Run **specific tag** in test_data_1.txt and test_data_2.txt
          * run.py -i "tag name" Common_Cases\Common_testcase.txt Ford\02_Connection.txt



