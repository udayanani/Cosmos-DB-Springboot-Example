## Overview
This sample project demonstrates how to use Azure CosmosDB via Spring Boot Starter `azure-cosmosdb-spring-boot-starter` to store data in and retrieve data from your Azure Cosmos DB.

## Prerequisites

* An Azure subscription; if you don't already have an Azure subscription, you can activate your [MSDN subscriber benefits](https://azure.microsoft.com/en-us/pricing/member-offers/msdn-benefits-details/) or sign up for a [free Azure account](https://azure.microsoft.com/en-us/free/).

* A [Java Development Kit (JDK)](http://www.oracle.com/technetwork/java/javase/downloads/), version 1.8.

* [Apache Maven](http://maven.apache.org/), version 3.0 or later.

## Quick Start

### Create an Azure Cosmos DB on Azure

1. Go to [Azure portal](https://portal.azure.com/) and click +New .
2. Click Databases, and then click Azure Cosmos DB to create your database. 
3. Navigate to the database you have created, and click Access keys and copy your URI and access keys for your database.
                                                                                                                                  
### Config the sample

1. Navigate to `src/main/resources` and open `application.properties`.
2. replace below properties in `application.properties` with information of your database.
   ```properties
   azure.cosmosdb.uri=your-cosmosdb-uri
   azure.cosmosdb.key=your-cosmosdb-key
   azure.cosmosdb.database=your-cosmosdb-databasename
   ```

### Run the sample

1. Change directory to folder `azure-cosmosdb-spring-boot-sample`.
2. Run below commands. 
 
   - Use Maven 

     ```
     mvn package
     java -jar target/azure-ducumentdb-spring-boot-sample-0.0.1-SNAPSHOT.jar
     ```

  
