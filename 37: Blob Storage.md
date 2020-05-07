# Reading 37: Blob Storage
## MS Docs: Introduction to Blob Storage
- Blob storage is designed for:
  - Serving images or documents directly to a browser
  - Storing files for distributed access
  - Streaming video and audio
  - Writing to log files
  - Storing data for backup and restore, disaster recovery, and archiving
  - Storing data for analysis by an on-premises or Azure-hosted service
  
### Blob Storage Resources
- The storage account
- A container in the storage account
  - Name must be lowercase
- A blob in a container

## MS Docs: Quickstart: Azure Blob storage client library v12 for .NET

### Set up
- Create project, install package, set up app framework, copy credentials into Azure portal, configure storage connection string

### Code Examples
- Get connection string
- Create a container
- Upload blobs to a container
- List the blobs in a container
- Download blobs
- Delete a container
