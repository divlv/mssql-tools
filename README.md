# mssql-tools

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