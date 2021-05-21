# mssql-tools

[![Build Status](https://img.shields.io/docker/cloud/build/emergn/mssql-tools)](https://hub.docker.com/r/emergn/mssql-tools)
[![Docker Automated build](https://img.shields.io/docker/cloud/automated/emergn/mssql-tools)](https://hub.docker.com/r/emergn/mssql-tools)
[![Docker Image Size](https://img.shields.io/docker/image-size/emergn/mssql-tools/latest)](https://hub.docker.com/r/emergn/mssql-tools)


SQL Server Command Line Tool on Alpine Linux. Added all the necessary libraries, e.g. *libcurl*.

# Usage

Default run for sqlcmd help:

```bash
docker run emergn/mssql-tools
```

Example connect to SQL server:
```bash
docker run -it emergn/mssql-tools -S <hostname> -U <username>
```

Example connect to Azure SQL server, using Azure Active directory authentication:
```bash
docker run -it emergn/mssql-tools -S azuredatabase.database.windows.net -d azuresqldbname -U AADuser@example.com -P SecUrEpAsSwOrd -G
```

eof