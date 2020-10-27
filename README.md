Sizing an Elastic Pool eDTU and Storage resources
=================================================

            
This runbook sizing an elastic pool set Maximum DTUs utilized by all databases in the pool  . And set Maximum storage bytes utilized by all databases in the pool. You can look up the available
 characteristics and tiers on [https://docs.microsoft.com/en-us/azure/sql-database/sql-database-elastic-pool](https://docs.microsoft.com/en-us/azure/sql-database/sql-database-elastic-pool) 


This runbook takes the following parameters:


 
ResouceGroupName: The name of the resource group that the SQL server is part of.
 


ServerName: The SQL server name.
 


ElasticPoolName: Specifies the name of the elastic pool.
 


Dtu: Specifies the total number of shared DTUs for the elastic pool. The default values for different editions are as follows: - Basic. 100 DTUs

 


DatabaseDtuMin: Specifies the minimum number of DTUs that the elastic pool guarantees to all the databases in the pool. The default value is zero (0).


DatabaseDtuMax: Specifies the maximum number of DTUs that any single database in the pool can consume. The default values for different editions are as follows: - Basic. 5 DTUs



Edition: Specifies the edition of the Azure SQL Database for the elastic pool. You cannot change the edition. The acceptable values for this parameter are:- None


SubscriptionID: An optional subscription ID if you want to work against an Azure subscription. The default is subscription is selected if not set. ** *** *


 


![Image](https://github.com/azureautomation/sizing-an-elastic-pool-edtu-and-storage-resources/raw/master/sizing-azuresqldb-elasticpools.png)


** *** *


 


** *** *

        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
