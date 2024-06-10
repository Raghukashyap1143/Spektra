# Exercise 2: Use MySQL Workbench To Connect To Your Pre-Created RDS (Aurora) Instance.
In this exercise, you will be connecting your pre-created RDS (Aurora) Instance using the **MySQL Workbench Application**.
1. Open the **MySQL Workbench Application** on the LabVM, and on the MySQL Workbench homepage, click on the plus icon to add a new database connection.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/OPENMYSQL.png)
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/newcon.png)
2. Provide the below details in the opened **Setup New Connection** dialog box:
+ For the Connection Name, enter **Aurora**.
+  For the Username, enter
+  For the Hostname, enter cluster endpoint
+  For the Password, click on **Store in Vault** and enter , and then click **OK**.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/aurora.png)
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/pass.png)
3. Click on **Test Connection** to verify whether the connection with MySQL is successful or not, and then click **OK**.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/testcon.png)
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/testconnectionpopup02.png)
4. Click **OK** to save the connection details and verify that the connection is named **Aurora**.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/save01.png)
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/aurora01.png)
5. Double click on connection **Aurora** to open a **Query Editor**.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/aurora01.png)
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/queryeditor02.png)
6. In the Query Editor, execute the following query to verify that no data exists in your Aurora instance.

```Select * from mydb.employee;```
You should receive a message showing that mydb.employee does not exist.

![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/output01.png)


<question source ="https://raw.githubusercontent.com/Raghukashyap1143/Spektra/main/Interns-Lab-Onboarding-Raghavendra_Prasad_K/Question1.md" />
<question source ="https://raw.githubusercontent.com/Raghukashyap1143/Spektra/main/Interns-Lab-Onboarding-Raghavendra_Prasad_K/Question2.md" />

