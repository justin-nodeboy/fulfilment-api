### Status
[![Build Status](https://travis-ci.org/Epic-Software-Solutions/fulfilment-api.png)](https://travis-ci.org/Epic-Software-Solutions/fulfilment-api)
# fulfilment-api
Fulfilment API

The API provides the following services

* Create/Edit/Delete Fulfilment workflows
* Create/Edit/Delete Webservice integrations
* Manage orders from the market
* Approve orders from the market (where required)
* Process orders via the workflow engine
* Call external API's defined in Web Service Configurations

## Pre-requisites

### Desktop
![MyGet tenant](https://img.shields.io/badge/dotnetcore-2.0.3--sdk-green.svg?longCache=true&style=for-the-badge)

You will need .net core, which is used to host and build the api. You can install .net core by going here:

[Install dotnet core](https://www.microsoft.com/net/learn/get-started)

***
### Server
Your server will need to have Docker installed. For ease we recommend [Digital Ocean](https://www.digitalocean.com) as they have excellent deals on droplet hosting (from as little as $5/month).

[Contact us](www.epic-software.co.uk) if you would like to look at our hosted plans, or for support.

An individual host does not require massives amounts of ram or compute power, however scale the server size for your needs. The application stack can also be load balanced.

#### Environment Variables
You will need to set the following Environment Variables:

`SQL_CONNECTION` - This contains your SQL connection string

`ASPNETCORE_URLS` - For development, set this to `http://localhost:5000`

`ASPNETCORE_ENVIRONMENT` - For development, set this to `Development`
***
### Database
You will need a SQL database for the fufilment engine. You can use any of the database providers below. The full list of EntityFramework Core providers can be found [here](https://docs.microsoft.com/en-us/ef/core/providers/), submit a PR to add another provider.

* SQL Server 2008 onwards
* PostgreSQL
* MySQL


