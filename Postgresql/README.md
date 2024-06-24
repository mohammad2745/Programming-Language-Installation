## Install Postgres and pgAdmin process

### Install Postgres

```sh
sudo apt update
```

```sh
sudo apt install gnupg2 wget nano
```
<p>Add the PostgreSQL 16 repository</p>

```sh
sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list
```

```sh
sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list
```

```sh
sudo apt update
```

<p>Install PostgreSQL 16</p>

```sh
sudo apt install postgresql-16 postgresql-contrib-16
```

Start and enable PostgreSQL service

```sh
sudo systemctl start postgresql
```

```sh
sudo systemctl enable postgresql
```

```sh
sudo systemctl restart postgresql
```

Check Version

```sh
psql --version
```

Stop PostgreSQL service

```sh
sudo service postgresql stop
```

<p>Connect to PostgreSQL</p>

Connect as the postgres user

```sh
sudo -u postgres psql
```

Set a password for postgres user

```sh
ALTER USER postgres PASSWORD 'password';
```

To exit out of the PostgreSQL prompt

```sh
\q
```

```sh
quit
```

### Install pgAdmin

```sh
curl -fsS https://www.pgadmin.org/static/packages_pgadmin_org.pub | sudo gpg --dearmor -o /usr/share/keyrings/packages-pgadmin-org.gpg
```

```sh
sudo sh -c 'echo "deb [signed-by=/usr/share/keyrings/packages-pgadmin-org.gpg] https://ftp.postgresql.org/pub/pgadmin/pgadmin4/apt/$(lsb_release -cs) pgadmin4 main" > /etc/apt/sources.list.d/pgadmin4.list && apt update'
```

<p>Install for both desktop and web modes </p>
```sh
sudo apt install pgadmin4
```

<p>Install for desktop mode only </p>
```sh
sudo apt install pgadmin4-desktop
```

<p>Install for web mode only </p>
```sh
sudo apt install pgadmin4-web 
```
