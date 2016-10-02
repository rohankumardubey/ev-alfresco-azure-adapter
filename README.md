# Alfresco adapter to work with Azure block storage
# Initial version developed by the EisenVault development team. Reach us at contact@eisenvault.com
# Initial commit on 1st October 2016

#Credits
Base Code taken from Ryan Berg's repository: https://github.com/rmberg/alfresco-s3-adapter
Modified the above code to work with Azure.


#Disclaimer
We have done basic testing and it seems to work - would appreciate your help in testing it further.
Pull Requests / Issues / Contributions are welcome!
 
#Build Instructions

 * After cloning the project, run `mvn clean install` to download dependencies and build the project

Installation / Configuration

 * After installing the `alfresco-azure-adapter.amp` package you will need to add some properties to your `alfresco-global.properties` file:
 
```
# Your Azure credentials

azure.accessKey=hUemXw0sD8e72/E5JrQZEFelkOG19icdmEU9hTfov8XmAPjGl0oX5l3/qzghHi+5Zj9tp4zC96ZX+B7Yz2wOVQ==

# The Azure block content store Container Name
azure.containerName=alfresco-docs-2

# The Azure block content store Account Name
azure.accountName=evvipuldev

# The relative path within the bucket to use as the content store
dir.contentstore=contentstore

# The relative path within the bucket to use as the deleted content store
dir.contentstore.deleted=contentstore.deleted