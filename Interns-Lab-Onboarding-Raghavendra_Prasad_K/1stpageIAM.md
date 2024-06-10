# Getting started with AWS Identity And Access Management 
##### Follow the steps below to get started with the lab:

**1.Sign in to your AWS management Console:** Login to yous AWS Account using your credentials.

![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/managamentconsolelogin.jpg)

**2.Login to the Account by entering the UserName/Email**

![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/LoginPage.jpg)

**3.Continue by enter the password to complete the Signin**
![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/Passowrd.jpg)

**4.Once the login is Successful You will be redirected to AWS Dashboard**
![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/Dashboardservices.jpg)

___
# Introduction to AWS Identity And Access Management 
### LabDuration: 1 Hour
## Overview:
**What is IAM?**
AWS Identity and Access Management (IAM) is a web service that helps you securely control
access to AWS resources. With IAM, you can centrally manage permissions that control which AWS
resources users can access. You use IAM to control who is authenticated (signed in) and authorized
(has permissions) to use resources.
___

## Key Learnings:
In this hands-on lab, you will be learning the following:
* Understanding **AWS Identity And Access Management** Dashboard and its features
* Learn about differnt **Type of Policy**
* Create Customised Policies
* Learn to create **IAM users** and Managing IAM user by Policies
* Learn to create IAM groups and Adding Users into Groups
* Attaching **Inline policies** to IAM users and groups
* Deep-dive into understanding **Role** and Creating a Role 
___
## Hands-on Labs
* [Exercise 1:](#exploring-different-features-of-policy-and-there-types) Exploring Different Features of policy and there Types
* [Exercise 2](#exercise-2-creating-new-policy): Creating New Policy
* [Exercise 3](#exercise-3-creating-new-users-and-attaching-inline-policy): Creating New Users and attaching Inline policy
* [Exercise 4](#exercise-4-creating-new-groups-and-adding-users-to-groups): Creating New Groups and Adding users to groups 
* [Exercise 5](#exercise-5-creating-role-for-aws-servicesexercise-5-creating-role-for-aws-services): Creating Role For AWS services
___


# Exercise 1: Exploring Different Features of policy and there Types
This exercise will help you understand the concept of policy and various types of policies.

Policies are JSON documents in AWS that let you specify who has access to AWS resources, and what actions they can perform on those resources. You can attach a policy to an identity or resource to define their permissions. AWS evaluates these policies when the IAM principal makes a request. Permissions in the policies determine whether the request is allowed or denied.
**Different Types of Policies:**
* [AWS managed policy-Job function](#task-2-exploring-aws-managed-job-function-policies)
* [AWS managed Policy](#task-3-exploring-aws-managed-policies)
* [AWS Customer Policy](#task-1-creating-customer-managed-policies)

___

## Task 1: Exploring IAM Dashboard

1. To access the IAM dashboard via the AWS Dashboard, search "IAM" service in the search field.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/IAMselect.jpg)
2. After selecting "IAM" service, you will be redirected to the IAM Dashboard.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/IAMdash.jpg)
___
## Task-2: Exploring AWS managed-job function Policies
**What are AWS managed- job function?**
AWS managed policies for job functions are designed to closely align with common job functions in the IT industry. These policies allow you to grant the necessary permissions to carry out tasks expected of someone in a specific job role.
1. Click on **Policies** under Access management in IAM dashboard.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/policyclick.jpg)
2. Under **Filter by Type** dropdown Select for **AWS managed- job function**.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/AWSmanaged-jobfunction.jpg)
3. Explore Different AWS managed- job function policies Pre-defined by AWS.
____
## Task 3: Exploring AWS managed Policies
**What are AWS managed policies?**
AWS managed policies are standalone policies that are created and administered by AWS1. They have their own ARNs that include the policy name. They are a collection of policies that make managing permissions as easy as possible2. They can be applied across the entire scope of specific AWS resources.

1.Under **Filter by Type** dropdown Select for **AWS managed**.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/AWSmanaged.jpg)
2. Explore Different AWS managed policies Pre-defined by AWS.
___

# Exercise 2: Creating New Policy
## Task 1: Creating Customer managed policies:
**What are Customer managed Policies?**
A customer-managed policy is a critical component of AWS cloud security. It allows customers to define and enforce fine-grained permissions to access various AWS services and resources.
1.Click on **"Create policy"**
![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/createpolicytoggle.jpg)
2.Select the **service** you intend to apply restrictions and set the policy editor to **Visual** for beginner-friendly operation.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/createpolicyservice.jpg)
3.Select whether the policy should **allow or deny**.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/EC2policyACtions.jpg)
4. Choose the actions to be performed.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/denyruninstance.jpg)
5. Define the **resources**.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/defineresources.jpg)
6. Conditions can be added to have fine grained restriction by clicking on **"Add another condition"**
![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/Createanewcondition.jpg)
7. Select the apporiate values from the dropdows and enter the **Value**. Once complete click on **Add Condition**.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/condition.jpg)
8. You can review the policy template by changing the policy editor to JSON.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/JSON.jpg)
9. Click on **"next"** once the policy is defined.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/policynextbutton.jpg)
10. Name the policy template under **"Policy Name"**.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/policyname.jpg)
11. Click on **"Create policy"** once complete
![alt text](https://iamguidessqwerty.s3.amazonaws.com/SS/createpolicyfinal.jpg)
____
Custom Policy can be reviewed under **"Filter by Type"** dropdown and selecting **"customer policy"**
___

# Exercise 3: Creating New Users and attaching Inline policy

An IAM user is an identity within your AWS account that has specific permissions for a single person or application. Users can be organized into groups that share the same permissions.
## Task 1: Creating IAM User
1. Navigate to Users in IAM console by clicking on **"Users"**
![alt text](https://iamguidessqwerty.s3.amazonaws.com/users/UsertoggleIAM.jpg)
2. Click on **"Add User"**.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/users/Clickcreateuser.jpg)
3. Enter **User Details** like **"User Name"** and fill the check box of **"Provide user access to the AWS Management Console"**
![alt text](https://iamguidessqwerty.s3.amazonaws.com/users/checkbox_name.jpg)
4. Fill the check box containing **"I want to create an IAM user"**
![alt text](https://iamguidessqwerty.s3.amazonaws.com/users/IwanttocreateIAMuser.jpg)
5. Choose the preffered checkbox for password authentication.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/users/autogeneratepassword.jpg)
6. Click on **"Next"**.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/users/clicknext.jpg)
7. Choose the permission options to **"Attach policies directly"** to attached **"customer policy"** created earlier.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/users/Attachpolicy.jpg)
![alt text](https://iamguidessqwerty.s3.amazonaws.com/users/customerpolicy.jpg)
8. Set **"Permission Boundaries"** if Necessary.(i.e, Set a permissions boundary to control the maximum permissions for this user. Use this advanced feature used to delegate permission management to others)
![alt text](https://iamguidessqwerty.s3.amazonaws.com/users/permissionboundaries.jpg)
9. Click **"Next"**
![alt text](https://iamguidessqwerty.s3.amazonaws.com/users/clicknext1.jpg)
10. Review the User details and click on **"Create User"**.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/users/review.jpg)
11. Download the ".csv" file of the user crediantials to Login as IAMUser. 
![alt text](https://iamguidessqwerty.s3.amazonaws.com/users/download.jpg)
___
## Task 2: Create inline policy for a User

1. Navigate to user panel. And click on the user
![alt text](https://iamguidessqwerty.s3.amazonaws.com/inlinepolicy/userdetails.jpg)
2. Under **"Add permissions"** , Click on **"Create Inline"** policy.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/inlinepolicy/createinline.jpg)
3. Follow the same steps used to create a customer policy with user needs.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/inlinepolicy/similarsteps.jpg)
4. Click **"Next"**.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/inlinepolicy/clicknext.jpg)
5. Provide a **"policy Name"** and Review the policy, Once Reviewed click On **"Add permissions"**.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/inlinepolicy/createpolicy.jpg)

___

# Exercise 4: Creating New Groups and Adding users to groups

In AWS IAM (Identity and Access Management), you can create groups to easily manage permissions for sets of users. Here's how you can create a new group and add users to it.

## Task 1: Creating New Group

1. Navigate to **"User groups"** in IAM Dashboard.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/usergroups/IAMdashboard.jpg)

2. Click on **"Create Group"** under usergroups.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/usergroups/creategroupbutton.jpg)

3. Provide a name for the group under **"User Group Name"** And Also select the User that you want to attach to the group in **"Add user to group"** Section.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/usergroups/Givenameandselectusers.jpg)

4. Select the **Policy** that you want to attach to the Group. All the users in this groups inherits the same Policy attached.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/usergroups/attachpolicy.jpg)

5. Click on **"Create User Groups"** to complete the process.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/usergroups/click.jpg)

6. Once the group is successfully created you will be able to view them and also modify users and permission.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/usergroups/successful.jpg)

___

# Exercise 5: Creating Role For AWS servicesExercise 5: Creating Role For AWS services

An IAM role is an identity you can create that has specific permissions with credentials that are valid for short durations. Roles can be assumed by entities that you trust.

## Task 1: Creating New Role 

1. Navigate to **"Roles"** from IAM Dashboard.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/roles/navigate.jpg)

2. Click on **"Create Role"** to create a new role or AWS pre-defined roles can be used.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/roles/create+role.jpg)

3. Choose the **Trusted Entity Type**.[AWS offers different trusted entities for roles. Common options include AWS service, another AWS account, or an identity provider (like AWS Cognito or SAML). Choose the appropriate trusted entity for your use case.]
![alt text](https://iamguidessqwerty.s3.amazonaws.com/roles/trustedentity.jpg)

5. From the dropdown select the Use case i.e, the service type.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/roles/usecase.jpg)

6. Click on **"Next"**
![alt text](https://iamguidessqwerty.s3.amazonaws.com/roles/next.jpg)

7. Attach policy to the role to Finegrate restriction allowing only to have required permission Under **"Set Permissions"**. Once Permissions are attached Click on Next.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/roles/permission.jpg)

8. Provide a **Name and Description** on the Role That you want to create
![alt text](https://iamguidessqwerty.s3.amazonaws.com/roles/name.jpg)

9. Review the trusted enitity, the policy and Click **"Create role"**.
![alt text](https://iamguidessqwerty.s3.amazonaws.com/roles/create.jpg)
___
**Congratulation You have successfully Completed on Understanding How IAM is Used to create role,users,groups and Also to create Policies.
With this, you have completed all the exercises.**
