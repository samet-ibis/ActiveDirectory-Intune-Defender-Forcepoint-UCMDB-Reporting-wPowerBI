# ActiveDirectory-Intune-Defender-Forcepoint-UCMDB-Reporting-wPowerBI
This repository explains how can u create your own reports for AD, Forcepoint, Intune and Defender with PowerBI. And includes a PowerBI sample (.pbit)
This sample file have some of reports like;
Installed Apps on Devices, BitLocker Status, Defender Alarm Status and Trend, Email Security Reports, Devices on your Active Directory, Intune, Defender and Forcepoint
AV Status, Onboarding Status on Defender, Exposure and Risk Scores for your devices and much more than. Also you can run your own KQL queries for Defender reports on this sample file.


🎯Intune

You have 2 methods for getting data from Intune; <br />

⭕Method 1; <br />
          ⧁ There is a table here in the PowerBI sample named deviceManagement-intunewithazureapp<br />
          ⧁ This table runs a query with Azure Application informations and going to getting data from Intune with Microsoft Graph. And it does it without an username or password, it does with your app informations.<br />
          ⧁ When the parameters box appears, just type your own App ID, App Secret and Tenant ID.
          ⧁ Also you can use second method for getting data from Intune but i saw different values so i just put them into sample file.<br />
          ⧁ You can see which Intune Graph query references what here;<br />
          ⧁ https://learn.microsoft.com/en-us/graph/api/resources/intune-graph-overview?view=graph-rest-beta<br />
          ⧁ Also you can get more information about this query from here;<br />
          ⧁ https://www.linkedin.com/pulse/story-powerbi-microsoft-graph-api-service-side-refresh-journaux/<br />
           
⭕Method 2;<br />
          ⧁ It is very simple to get data with this method.<br />
          ⧁ Just get your own Data Warehouse URL and paste it to parameters box.<br />
          ⧁ It needs a username and password with read permissions to intune. <br />
          ⧁ If you want to create your own pbix, u can reference this document;<br />
          ⧁ https://jannikreinhard.com/2022/07/10/build-powerbi-dashboard-based-on-intune-data-warehouse/ <br />
           
Requirements;<br />

⭕Method 1;<br />
          ⧁ You need an Azure App with api permission to these permissions;<br />
            ![azureapp](https://user-images.githubusercontent.com/100233276/203585136-1f3ec6dc-e1fa-455a-9251-f5df5ddf660b.PNG)<br />
          ⧁ Note: This permissions are extended for my lab but you dont have to give this all permissions to your app. <br />
          ⧁ It changes for what u want or which you want to get data from Graph. <br />
          ⧁ You can also follow this steps at link above (Method 1). <br />

⭕Method 2;<br />
          ⧁ You need your own Data Warehouse URL. <br />
          ⧁ A user who has permissions to read all intune data. <br />
          
🎯Defender <br/>
          ⧁ There is a function available on Power Query Editor named AdvancedHuntingQuery.<br />
          ⧁ It is very simple, just paste your own Advanced Hunting query to this function and get your data to new table you change as you want.<br />


Requirements; <br />
          ⧁ U need an account with permissions to Security Operator, Security Administrator or Global Admin. <br />
          
🎯Forcepoint <br/>
          ⧁ You need to know your own Forcepoint database address. <br />
          ⧁ A user who has permissions to read wbsn-data-security database tables. <br />
          ⧁ When the parameters box appears, just type your forcepoint sql database address.
          ⧁ Note that: this SQL query doesn't harmfull for your database tables. They just simple SELECT queries.
          
🎯Active Directory <br/>
          ⧁ You need an account with permissions to read all devices on your Active Directory.
          ⧁ When the parameters box appears, just type your domain name (contoso.com) and be sure that u can access your DCs with LDAP ports. 

Don't hesitate to contact with me, this README file is for person who has information about this things. I can help you for your reports. Just send me an email.  <br />
E-Mail: asametibis@gmail.com  <br />
More information will be come next weeks.

!!!!New Release for MAM (Mobile Application Management) report🙌
![image](https://github.com/t0neex/ActiveDirectory-Intune-Defender-Forcepoint-UCMDB-Reporting-wPowerBI/assets/100233276/f904adc3-f12e-4841-a659-c3f867edd798)




![activedirectory](https://user-images.githubusercontent.com/100233276/226177721-7a09a55a-3fd1-48f8-98e4-d416abcf3441.PNG)

![msdefenderdetailed](https://user-images.githubusercontent.com/100233276/226177788-c2b6524c-c47e-465f-b13c-be881011ffa9.PNG)
![MSDefenderEmailSec](https://user-images.githubusercontent.com/100233276/226177791-dca1f78b-b22c-4ac4-af86-fbcab5d76a89.PNG)
![ucmdb](https://user-images.githubusercontent.com/100233276/226177794-cf641c11-5b1a-4f8d-8486-c088b9928755.PNG)
![bitlocker](https://user-images.githubusercontent.com/100233276/226177798-3e4a4d2b-5c4c-4c1a-8581-be9e6353d021.PNG)
![forcepoint](https://user-images.githubusercontent.com/100233276/226177802-66b9724e-6c9c-4b1f-8090-3f1fd3734471.png)
![installedappsdefender](https://user-images.githubusercontent.com/100233276/226177805-a5d28ce2-abc5-444e-b4a1-18882868c345.PNG)
![intune](https://user-images.githubusercontent.com/100233276/226177806-bdb20449-b103-4eb1-8278-99795655c677.PNG)
![MSDefender](https://user-images.githubusercontent.com/100233276/226177808-4601f22d-da7a-4fe8-b84b-bf8d8c8072c2.PNG)
![MSDefenderAlarmTrend](https://user-images.githubusercontent.com/100233276/226177811-7c6e26e1-4fd3-4a7c-9912-e580a5fa3efa.PNG)
