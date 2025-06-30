# Data Architect Procedure for Scalable Physical Plans and Database Design Deployment with ER-Studio

In this discourse, we show an infographic procedure by which Data/Database Architects can deploy a scalable Physical Data Model (PDM),  and deploy the PDM on a Database. ER/Studio is used for the design procedures outlined in this discourse. Microsoft SQL Server 2022 is used as the database for deployment. 

For completeness, it is advisable that Developers that intend to use the procedures outlined here should first complete and fully understand the procedures for designning Logical Data Models (LDMs) outlined here: https://github.com/manuelbomi/Data-Architect-Procedure-for-Designing-a-Scalable-Logical-Data-Model-with-ER-Studio 

### Procedure
---
> [!IMPORTANT]
> To the Developer: If Microsoft SQL Server is the intended database for deploying the PDM, it is advisable to use MS SQL Server Authentication method (with 'sa' as User Name and password as 'your_very_strong_password') instead of the Windows Authentication method. ER/Studio readily works with MS SQL Server Authentication method more than the Windows Authetication method.
> A very short video that explains how to configure the MS SQL Server Authentication method is available here: https://www.youtube.com/watch?v=-UY0fHckkGc
> 
--- 

#### Start with procedures for creating a Logical Data Model here: https://github.com/manuelbomi/Data-Architect-Procedure-for-Designing-a-Scalable-Logical-Data-Model-with-ER-Studio. If the MS SQL Server database engine is the intended target, then ensure that the database is running and ensure that the authentication method is the MSSQL Server Authentication method. An infograph of a running MSSQL Server is shown below:
---
![Image](https://github.com/user-attachments/assets/b9c361ab-b2d2-4d12-b8c0-c743831f8265)


---
#### Start from the logical model. Load the LDM

![Image](https://github.com/user-attachments/assets/64388926-dbce-49d5-b110-c7129647840d)

---
#### Navigate to Data Dictionary

![Image](https://github.com/user-attachments/assets/2c55fb69-0c83-41a0-80c8-cb2e1cbdbf07)
---

#### Click Naming Standards Template and select New Naming Standards Template

![Image](https://github.com/user-attachments/assets/7b119ca5-397c-458a-97dc-140b61414bb7)

---

#### Give the naming template any desired name
![Image](https://github.com/user-attachments/assets/43a04da0-2955-4dbf-9fd8-4ee55fded228)
---

#### Click on  'Physical' button and change the Entity parameters as desired. You can change it to UPPER lower UpperCase etc
![Image](https://github.com/user-attachments/assets/31eb2f20-fa9e-4575-bb96-3614c15340fe)
![Image](https://github.com/user-attachments/assets/a0bc41e2-8e42-487d-b0bd-d32a3d9c8261)

---
#### Navigate to 'Mapping' and select the appropriate tab to replace any character with an underscore
![Image](https://github.com/user-attachments/assets/1a9aff44-66f4-4fd3-b8ce-5392704c329b)

---
#### Under ‘Binding Information’ select ‘Entity’ and select all. Click OK
![Image](https://github.com/user-attachments/assets/f147bc74-b663-4c9d-bc1e-fc715a526f80)

---

#### Navigate back to the Data Model page
![Image](https://github.com/user-attachments/assets/ca41ec57-f61f-4596-ad18-35927e2e2d3a)

---
#### Right click on the 'Main Model and select 'Naming Standard Utility'
![Image](https://github.com/user-attachments/assets/81a25d1a-184a-4bdf-aa40-edb2713c732b)

---
#### Select 'All' under 'Options'
![Image](https://github.com/user-attachments/assets/5949bba3-9301-4241-9176-628f3397b42f)

---
#### Select the named (naming) template and ensure that both Source and Target are selected for Logical
![Image](https://github.com/user-attachments/assets/212b6d74-4d81-4fc4-b4df-b97262f3fff2)

---
#### Select 'Run Translation' and press OK
![Image](https://github.com/user-attachments/assets/32107f2f-f11d-457c-831e-c50a435e4f48)

---
#### Select 'Run Translation'
![Image](https://github.com/user-attachments/assets/1adef587-d371-45fa-a45c-be5c1512cb70)

---
#### Right click on the model and pick 'Generate Physical Model'
![Image](https://github.com/user-attachments/assets/362571f0-5e6d-4c39-aadd-bf4253af4a32)

---

#### Give the physical model a name, pick Relational Database and select MS SQL Server
![Image](https://github.com/user-attachments/assets/fc2c8b39-f07b-4746-99a3-34d348027903)

---

#### Select all table, views etc
![Image](https://github.com/user-attachments/assets/d8e4f0cd-8f3b-47b3-8af7-ad0cebb87106)

---

#### Click next and select your naming template
![Image](https://github.com/user-attachments/assets/96833f4d-b514-4397-b435-c2112aeecfc6)

---
#### Give the tables and indexes names
![Image](https://github.com/user-attachments/assets/1e598df8-6a23-4646-86d5-0e572866b35d)

---
#### Give the tables and indexes names
![Image](https://github.com/user-attachments/assets/4b6320a4-624e-4f52-8548-8672bc901d3d)

---
#### Click Next
![Image](https://github.com/user-attachments/assets/c8d559ab-8e7f-4019-9d4d-019b7c8ed844)

---
#### The physical model will now exist at the lower end of the Data Model page
![Image](https://github.com/user-attachments/assets/7bc83664-3b36-4893-98d9-77eaebcb9ca7)

---
#### Right click on the physical model and click Generate Database
![Image](https://github.com/user-attachments/assets/5969b5c0-e780-44f0-9052-b9b38a86a210)

---
#### Select object with database connection and click Connect
![Image](https://github.com/user-attachments/assets/aeda7ace-8075-4e2c-8f3b-c48865e2ae45)

---

#### Select object with database connection
![Image](https://github.com/user-attachments/assets/fde69ab2-af31-4762-909d-1966c2de5bb6)

---

#### Select database parameters and ensure that the database server_connection name matches that of the MSSQL database
![Image](https://github.com/user-attachments/assets/7bf8eb57-e197-4582-92db-b5a54e52630b)

---

#### Input  'sa' as username and input the password and click next
![Image](https://github.com/user-attachments/assets/547543fb-3723-4bd8-b7f5-f0e022bc3487)

---

#### Click next and click select or create a database
![Image](https://github.com/user-attachments/assets/35e89686-5a55-4139-b771-cea79309dd31)

---

#### We have chosen to create a database named ER_Studio_HR_Dbase
![Image](https://github.com/user-attachments/assets/937d6eb0-47c6-4559-be4c-e96f7fbcf4be)

---

#### Click next and select all
![Image](https://github.com/user-attachments/assets/c1a4b040-f67a-4ce9-82d3-8a357cfb6467)

---
#### 27 Click next and click finish
![Image](https://github.com/user-attachments/assets/7d81a289-0116-4ba1-9c31-8a378be3db72)

---
#### You can choose to save the result and close the wizard
![Image](https://github.com/user-attachments/assets/cdbf75df-9750-4365-86f4-ee804bc91af4)

---
#### MS SQL Server Database before refreshing
![Image](https://github.com/user-attachments/assets/870a020e-911a-4a4d-bd82-3aa656c26936)

---
#### The ER_studio_HR_Dbase have been created
![Image](https://github.com/user-attachments/assets/a6dcc441-2b1d-4eb0-8e2b-b60278d20f5d)

---

#### You can expand to see some of the entities and tables
![Image](https://github.com/user-attachments/assets/7351b377-b1d6-471b-bc08-e8d680901073)

---
Thank you for reading through

---

Author's Background

```

Author's Name:  Emmanuel Oyekanlu
Skillset:   I have experience spanning several years in developing scalable enterprise data pipelines, architecting enterprise data solutions,
data engineering, machine learning, NLP and LLM applications as well as deploying scalable solutions (apps) on-prem and in the cloud.
I can be reached through: manuelbomi@yahoo.com
Website:  http://emmanueloyekanlu.com/
Publications:  https://scholar.google.com/citations?user=S-jTMfkAAAAJ&hl=en
LinkedIn:  https://www.linkedin.com/in/emmanuel-oyekanlu-6ba98616
Github:  https://github.com/manuelbomi

```

[![Icons](https://skillicons.dev/icons?i=aws,azure,gcp,scala,mongodb,redis,cassandra,kafka,anaconda,matlab,nodejs,django,py,c,anaconda,git,github,mysql,docker,kubernetes&theme=dark)](https://skillicons.dev)



