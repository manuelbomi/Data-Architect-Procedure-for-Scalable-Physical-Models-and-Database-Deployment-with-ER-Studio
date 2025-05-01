# Data-Architect-Procedure-for-Scalable-Physical-Plans-and - Database-Design-Deployment-with-ER-Studio

In this discourse, we show an infographic procedure by which Data/Database Architects can deploy a scalable Physical Data Model (PDM),  and deploy the PDM on a Database. ER/Studio is used for the design procedures outlined in this discourse. Microsoft SQL Server 2022 is used as the database for deployment. 

Fpr completeness, it is advisable that Developers that intend to use the procedures outlined here should first complete and fully understand the procedures for designning Logical Data Models (LDMs) outlined here: https://github.com/manuelbomi/Data-Architect-Procedure-for-Designing-a-Scalable-Logical-Data-Model-with-ER-Studio 

### Procedure
---
> [!IMPORTANT]
> To the Developer: If Microsoft SQL Server is the intended database for deploying the PDM, it is advisable to use MS SQL Server Authentication method (with 'sa' as User Name and password as 'your_very_strong_password') instead of the Windows Authentication method. ER/Studio readily works with MS SQL Server Authentication method more than the Windows Authetication method.
> A very short video that explains how to configure the MS SQL Server Authentication method is available here: https://www.youtube.com/watch?v=-UY0fHckkGc
> 
--- 

#### Start with procedures for creating a Logical Data Model here: https://github.com/manuelbomi/Data-Architect-Procedure-for-Designing-a-Scalable-Logical-Data-Model-with-ER-Studio. If the MS SQL Server database engine is the intended target, then ensure that the database is running and ensure that the authentication method is the MSSQL Server Authentication method. An infograph of a running MSSQL Server is shown below:
---
![Image](https://github.com/user-attachments/assets/a6dcc441-2b1d-4eb0-8e2b-b60278d20f5d)

---
#### Start from the logical model. Load the LDM
![Image](https://github.com/user-attachments/assets/7351b377-b1d6-471b-bc08-e8d680901073)
![Image](https://github.com/user-attachments/assets/b9c361ab-b2d2-4d12-b8c0-c743831f8265)
![Image](https://github.com/user-attachments/assets/64388926-dbce-49d5-b110-c7129647840d)
![Image](https://github.com/user-attachments/assets/2c55fb69-0c83-41a0-80c8-cb2e1cbdbf07)
![Image](https://github.com/user-attachments/assets/7b119ca5-397c-458a-97dc-140b61414bb7)
![Image](https://github.com/user-attachments/assets/43a04da0-2955-4dbf-9fd8-4ee55fded228)
![Image](https://github.com/user-attachments/assets/31eb2f20-fa9e-4575-bb96-3614c15340fe)
![Image](https://github.com/user-attachments/assets/a0bc41e2-8e42-487d-b0bd-d32a3d9c8261)
![Image](https://github.com/user-attachments/assets/1a9aff44-66f4-4fd3-b8ce-5392704c329b)
![Image](https://github.com/user-attachments/assets/f147bc74-b663-4c9d-bc1e-fc715a526f80)
![Image](https://github.com/user-attachments/assets/ca41ec57-f61f-4596-ad18-35927e2e2d3a)
![Image](https://github.com/user-attachments/assets/81a25d1a-184a-4bdf-aa40-edb2713c732b)
![Image](https://github.com/user-attachments/assets/5949bba3-9301-4241-9176-628f3397b42f)
![Image](https://github.com/user-attachments/assets/212b6d74-4d81-4fc4-b4df-b97262f3fff2)
![Image](https://github.com/user-attachments/assets/32107f2f-f11d-457c-831e-c50a435e4f48)
![Image](https://github.com/user-attachments/assets/1adef587-d371-45fa-a45c-be5c1512cb70)
![Image](https://github.com/user-attachments/assets/362571f0-5e6d-4c39-aadd-bf4253af4a32)
![Image](https://github.com/user-attachments/assets/fc2c8b39-f07b-4746-99a3-34d348027903)
![Image](https://github.com/user-attachments/assets/d8e4f0cd-8f3b-47b3-8af7-ad0cebb87106)
![Image](https://github.com/user-attachments/assets/96833f4d-b514-4397-b435-c2112aeecfc6)
![Image](https://github.com/user-attachments/assets/1e598df8-6a23-4646-86d5-0e572866b35d)
![Image](https://github.com/user-attachments/assets/4b6320a4-624e-4f52-8548-8672bc901d3d)
![Image](https://github.com/user-attachments/assets/c8d559ab-8e7f-4019-9d4d-019b7c8ed844)
![Image](https://github.com/user-attachments/assets/7bc83664-3b36-4893-98d9-77eaebcb9ca7)
![Image](https://github.com/user-attachments/assets/5969b5c0-e780-44f0-9052-b9b38a86a210)
![Image](https://github.com/user-attachments/assets/aeda7ace-8075-4e2c-8f3b-c48865e2ae45)
![Image](https://github.com/user-attachments/assets/fde69ab2-af31-4762-909d-1966c2de5bb6)
![Image](https://github.com/user-attachments/assets/7bf8eb57-e197-4582-92db-b5a54e52630b)
![Image](https://github.com/user-attachments/assets/547543fb-3723-4bd8-b7f5-f0e022bc3487)
![Image](https://github.com/user-attachments/assets/35e89686-5a55-4139-b771-cea79309dd31)
![Image](https://github.com/user-attachments/assets/937d6eb0-47c6-4559-be4c-e96f7fbcf4be)
![Image](https://github.com/user-attachments/assets/c1a4b040-f67a-4ce9-82d3-8a357cfb6467)
![Image](https://github.com/user-attachments/assets/7d81a289-0116-4ba1-9c31-8a378be3db72)
![Image](https://github.com/user-attachments/assets/cdbf75df-9750-4365-86f4-ee804bc91af4)
![Image](https://github.com/user-attachments/assets/870a020e-911a-4a4d-bd82-3aa656c26936)


