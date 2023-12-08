# hw-project for hospital transparency-in-pricing
For my project i choice the data set of the hospital tansparency-in-pricing.
## what is the transarencn in pricing ?
Transparency in pricing in the context of hospitals refers to the practice of openly and clearly disclosing the costs associated with medical services, procedures, and treatments. The goal is to provide patients with clear information about the financial aspects of their healthcare so that they can make informed decisions.
## What is the business problem and solution
The Business problems for the transparency-in-pricing in hospital one of them is the medical insurance because different medical insurance cover different package so customer will have different cost!
so for this case there no good soultion only things can do is find the one insurence that cover the most nomral sick most people have.
## Requirment for this project
The requirement fot this project is find out which insurance in data set i find cover or pay the most money.
Requirement 2 is find out what class take more pay or covergy by insurence which is inpatient or outpatient.
Requirement 3 is find out which payer category pay more.
## Project process
My project will following the precess below and  this image come from my team.
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/c39afe14-eb0d-420d-9331-312bf0f700f5)

## Data come from
when i choice this topic and understand the business problem , process and requiremtn in go find a data in the websit in www.dolthub.com The url for the data is https://www.dolthub.com/repositories/piaskowna/transparency-in-pricing/data/main This what it look like before the webscript
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/dd8b41d3-53ed-4291-8397-eb37b200c1d2)
## Webscript
After i get the data set for my project i use webscript to get the data and the tool is use to do the webcsript is the python. the code is in the file i put. Also my coding is bad so the code is my professor help me to creat. after professor help me creat the code i use the code webscripe the data and upload to my azure storage account.
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/103fae05-d82c-4732-bd25-ef503c669132)
This is the storage account i creating in azure and it has two blob the hwproject on is contined orginal data hwproject 2 is the data after the data transfermation.
This is what inside of hwporject look like![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/7d000ffa-3b89-46c4-9ec1-58e1213d1702)

## First Schema
After i storge my data i use the tool called dbschema to creat my dimension module and the module i creat is in the folder schema.
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/787c8121-e004-49c0-941e-4c1863de0cca)
Thi was the dimension module before i did the cleanning so i have two module this first one .
## Data transforming
After the schema is creat i come to the data transforming stage in this part i try to using python code todo that so this was my code
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/042e5c33-28c9-4a9a-a05e-46c7c4f362a8)
In this code i get the data from my auzre storage account then print out to check the data type, and the null value it contin.
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/b39d35b5-c625-4416-9b5c-d9f638d0ca1b)
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/524e738f-4b70-4d51-9bb8-0db1130c5620)
Thre lot of null value so i use following code to check the sum of null value each columns it have
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/70911d70-ec93-4df6-8f0a-8ba11938ff8c)
So it was a lot so i need use another code to remove all null values.
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/a36ed28e-7dde-4107-a8c0-fe4a3148773d)
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/228f2bca-1a30-4999-a92a-698e25cb29a7)
That is code i use and the result i get is very good all the null values is gone data look clean.
So the last step is make connection to my data warhouse which is the azure synpa i creat this i will show after .
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/ed8120d9-4040-4beb-abf0-c3ac25673264)
This code i get from professor that creat the connection to my datawarhouse very thinkful fo him to help me out 
after connection is start and good i try to insert my data in to datawarhouse and creat table but i fail it get my to erroy
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/225fe1da-cc5f-4a69-ac7f-141c632ed59c)
I ask professor this is type erroy this mean my data type is not match in both plase so i go to my data warhouse to check what  is happen and the following image is the azure synapa i create:
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/ab0e6186-b2e6-4c73-b08e-dfbda9025ca2)
you can see i creat three fact table is because i chage data type many time to check which data type it get wrong but you can see it was fail even i match both place data type 
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/44a086f8-61b3-4b55-8028-bc6af1df7705)
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/0047b721-a265-41f1-920b-3d9c4baeb6ee)
So the python code is fail then i ask one of my classmate Natalia to help use data pipline in the azure synap to do the data transfer i very thankful because she use her own time to help me do the project also the professor and my team mate to they all help my project.
i follow each step she told me and we use the team do the scren share so to check do i do wrong or not. but the reaslout we get is not good i fail again.
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/c6b81030-3654-46a0-9d63-fac32de61c46)
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/ce5b703f-5932-4c6d-97f8-010fa74ee23e)
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/4d81f5f0-b187-4e84-9a4c-4530276b3c19)
![image](https://github.com/fuleichencis2300/hw-project/assets/121892294/08a5c7fb-aace-4ef2-b5da-bc36224073d9)

i cant fix this problem so is just use the data i clean in csv file to do the visual!.
## visual 





