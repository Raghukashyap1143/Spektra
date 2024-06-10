# Exercise 1: Connect To Your Source MySQL Database
In this exercise, you will be connecting your source **MySQL Database** hosted on the EC2 Windows Instance (LabVM) using the **MySQL Workbench Application.**
Follow the below steps to connect to your **MySQL Database** using the **MySQL Workbench Application:**
1. Open the **MySQL Workbench Application** on the LabVM, and on the MySQL Workbench homepage, click on the plus icon to add a new database connection.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/OPENMYSQL.png)
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/mysqlworkbenchpage.png)
2. Provide the below details in the opened Setup New Connection dialog box:
+ For the Connection Name, enter **Source**.
+ For the Username, enter
+ For the Password click on **Store in Vault**, and enter , and then click **OK**.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/connection.png)
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/pass.png)
3. Click on **Test Connection** to verify whether the connection with MySQL is successful and then click **OK**.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/testconnection.png)
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/testconnectionpopup.png)
4. Click on **OK** to save the connection details and verify that the connection is added with the name **Source**.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/save.png)
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/source.png)
5. Double click on connection **Source** to open a **Query Editor**.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/source.png)
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/queryeditor.png)
6. Go to the workbench and find the navigation pane on the left. Look for "schemas" and click on it. You'll see a database named "mydb." Under it, you'll find "Tables."
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/tables.png)
7. To load the data stored in the employee table, copy and paste the command given below, and then click on the execute button to run the query.

```Select * from mydb.employee;```
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/output.png)

<question source="https://raw.githubusercontent.com/Raghukashyap1143/Spektra/main/Inlinequestion/Question3.md"
/>




