# Exercise 6: Create A Database Migration Task
An AWS Database Migration Service (AWS DMS) task is where all the work happens. You use tasks to migrate data from the source endpoint to the target endpoint, and the task processing is done on the replication instance. You specify what tables and schemas to use for your migration and any special processing, such as logging requirements, control table data, and error handling.
Follow the below steps to create Database migration tasks.
1. In the left navigation pane, choose Database migration tasks and click on the **Create task**.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/dmstask01.png)
2. In the Task Configuration, provide the below values.
+ For the Task identifier, enter **MySQL-Aurora**.
+ For the Replication instance, choose the Replication instance that you have created in **exercise 3**.
+ For the Source database endpoint, choose the source endpoint that you have created in **exercise 4**.
+ For the Target database endpoint, choose the source endpoint that you have created in **exercise 5**.
+ For the Migration type, choose the option **Migrate existing data** from the drop-down menu
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/dmstask02.png)
3. Scroll down to the **Task Settings** and provide the below values.
+ For the editing mode, choose **Wizard**.
+ For the Target table preparation mode, choose **Do nothing**.
+ For the LOB column settings, choose **Do nothing**.
+ For the Data Validation, choose **Turn off**.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/tasksettings.png)
4. Scroll down to the **Table Mappings** and provide the below values.
+ For the editing mode, choose **Wizard**.
+ For the Selection rules, click on **Add new selection rule**.
+ For the schema, choose **Enter a schema**.
+ For the Source name, enter **%mydb**.
+ For other settings, keep everything **Defaults**.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/taskschema.png)
5. Scroll down to the Premigration assessment and select **disable Turn on premigration assessment**.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/turnoff.png)
6. Scroll down and click on **Create task**.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/createtask.png)
7. Wait for at least 5 minutes, and then verify that the status of the task is **Load complete**.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/loadcomplete.png)
8. Once the task status shows as **Load complete**, return to the **MySQL Workbench** and open the existing connection with the name **Aurora**.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/aurora01.png)
9. In the **Query Editor**, enter the below query and click on **execute**.
```Select * from mydb.employee;```
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/execute.png)
10. You will see that your mydb data has been migrated to your Aurora instance.
**Congratulations!** You have now successfully used the AWS Database Migration Service to migrate data from your source MySQL server to your target Aurora instance.






