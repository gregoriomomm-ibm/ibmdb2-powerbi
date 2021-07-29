# ibmdb2-powerbi
IBM DB2 - PowerBI config

Personnal: https://github.com/gregoriomomm/

Simple instructions to connect PowerBI to DB2 

1. Download DB2 Drivers, in this case I would be using [Windows 64 bits DB2 11.5](https://www.ibm.com/support/pages/download-initial-version-115-clients-and-drivers) ;
2. Unpack the contents, and Run AS ADMINISTRATOR, the setup.exe. This is importat to Run with the right privileges ;
3. To make sure that you ran correctly, look at c:\Windows\assembly and check if it has at least "IBM.Data.DB2" for your processor architecture ;
4. Optionally, you can you user this [testconn](https://www.ibm.com/docs/en/db2/11.5?topic=net-testconn-command) command to ensure that is correctly configured ;
5. Run PowerBI (I am using Version: 2.95.804.0 64-bit (2021 july)) ;
6. Select at the first screen "Get data from another source" and choose "IBM DB2 database" ;
7. Here you fill in the Server anda database information that you have including the port like db2w-your-server.db2w.cloud.ibm.com:50001 and your DB Name, like BLUDB ;
8. At advanced options, select the IBM Driver, as that was the one that you just downloaded and install it ;
9. Check if, for your case, you prefer to import new tables at the default option import, or directly run queries (Direct query) ;
10. Uncheck Navigate using full hierarchy and click ok ;
11. At this step, choose "Database" at the left panel and fill in User and password (look at the credential file for the username like bluadmin or for the username that you want, if you already customized a user, and password will be at a speciic tag called "password") ;

![image](https://user-images.githubusercontent.com/35934706/127484699-775c4f5f-b948-40b3-bbc5-785e14ebd674.png)

