# Adventure-Works-Data-Engineering-Project

Project Overview:

Business Requirements

Project Goals:


Project Architecture:
You can find the detailed information on the diagram below:

![image](https://github.com/user-attachments/assets/4778f411-3a0e-4e00-a863-69de45489d6b)


Dataset Used:



Technologies Used:

•	Data Source: GITHUB

•	Orchestration: Azure Data Factory

•	Transformation: Azure Databricks

•	Security: App Registrations

•	Storage: Azure Data Lake Gen2

•	Analytics: Azure Synapse Analytics

•	Data Visualization: PowerBI



Prerequisite:

• Azure account with active subscription

• Databricks community edition account

• Knowledge about storage account, dataframe, azure data factory, sql etc.


1.Initial Set-up:

• Create Azure account

• Create a Resource Group to house and manage all the Azure resources associated with this project.

• Within the created resource group,set up a storage account. This is specifically configured to leverage Azure Data Lake Storage(ADLS) Gen2 capabilities.

• Create a Container inside this storage account to hold the project's data. i.e, Bronze,Silver,Gold.


2.Data Ingestion using Azure Data Factory:

• Begin by creating an Azure Data Factory workspace within the previously established resource group.

• After setting up the workspace, launch the Azure Data Factory Studio.

• Upload the dataset from kaggle to GitHub.

• Within the studio, initialize a new data integration pipeline. Now use the Copy Data activity to move data efficiently between various supported sources and destinations.

• Configuring the Data Source with HTTP template as we are using http request to get the data from GitHub repo.

• Establishing the Linked Services for source(i.e, using Https).

• Configuring the File Format for and setting up the Linked Service Sink(i.e, Adls gen2).

• Repeat above steps to load all other datasets.

• You can connect all the copy data activity together and run them all at once.

• You can use Manual (or) Scheduled Trigger to run this Pipeline.




































