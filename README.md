# How to create a postgresql database in Ubuntu

## Install postgresql
```
sudo apt-get install postgresql
```

## Create user
```
sudo -u postgres createuser -P user
```

## Create database
```
sudo -u postgres createdb -O user mydb
```

## Connect
```
psql -d mydb -h localhost -U user
```

## Drop database
```
sudo -u postgres dropdb mydb
```

## Drop user
```
sudo -u postgres dropuser user
```

## Restart database
```
sudo /etc/init.d/postgresql restart
```

## Set connection parameters for pg
Name | Value
-----------|---------
PGHOST | localhost
PGDATABASE | mydb
PGUSER | user
PGPASSWORD | password
PGPORT | 5432
