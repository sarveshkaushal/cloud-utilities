# cloud-utilities
This repo contains projects that are build to help with cloud development.
###DynamoUtil is a utility class which can be used to import all records from a dynamo table to .csv file.
This can be used if you don't want to use Amazon data pipeline feature to export data from dynamo.
##Usage:
```
DynamoUtil util = new DynamoUtil(getDynamoDBClient());
File file = util.export("dynamo-table-name", "/tmp/");//tmp is temporary directory to store exported file
```
