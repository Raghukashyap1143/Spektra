# Exercise 3: Migrate your source MySQL database to your Aurora instance using the AWS Database Migration Service
In this exercise, you will use the AWS Database Migration Service to migrate your mydb database running on your MySQL instance to your Aurora instance.
Follow the below steps to migrate your source MySQL database to your Aurora instance using the AWS Database Migration Service
1. At the top of the AWS Management Console, in the search bar, search for the service DMS.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/dms.png)
2. On the AWS DMS page, open the navigation page on the left click on the **Replication Instance (1)**, and the **Create Replication Instance** (2).
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/replicate.png)
3. On the Replication Instance page, provide the below details to configure the Instance.
+ For the Replication Instance Name, enter replicationInstance.
+ For the Description, enter replicationInstance.
  ![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/createne.png)
+ For the Instance Class, choose **dms.t3.micro**
+ For the High Availability, choose **Dev or test workload(Single-AZ)**.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/dmst3.png)
+ For the Storage, enter **30**.
  ![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/storage.png)
+ For the Virtual private cloud (VPC) for IPv4, choose VPC name starting with **clgVpc**.
+ For the Public accessible, Deselect the option.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/ipv4.png)
+ Click on Create **Replication Instance**.
![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/createrep.png)
**Note: The creation of a replication instance may take 5-10 minutes. You may have to wait for your replication instance to become active.**
  ![alt text](https://docs-api.cloudlabs.ai/repos/raw.githubusercontent.com/CloudLabsAI-Azure/AustinCC/main/DMS/images/active.png)

  <question source ="https://raw.githubusercontent.com/Raghukashyap1143/Spektra/main/Interns-Lab-Onboarding-Raghavendra_Prasad_K/Question1.md" />
  










