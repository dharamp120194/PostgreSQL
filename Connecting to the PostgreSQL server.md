# Connecting to the PostgreSQL server

Specify the following parameters to connect to PostgreSQL:
- A host or host address
- A port
- A database name
- A user
- A password (or other means of authentication; but only if requested)

## Without specifying paramrters 

PostgreSQL looks for values set through enviroment variables, which are as follows:

- PGHOST or PGHOSTADDR
- PGPORT (set this to default 5432 if it is not set already)
- PGDATABASE
- PGUSER
- PGPASSWORD (Not recommended)

## Connection String 

```
psql "user=myuser host=myhost port=5432 dbname=mydb password=mypasswd"
```

Or use Uniform Resource Identifier (URI) format

```
psql postgresql://myuser:mypasswd@myhost:5432/mydb
```


