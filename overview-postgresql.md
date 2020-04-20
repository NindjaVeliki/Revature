# PostgreSQL

## Local install
### Windows
- Chocolatey: `choco install postgresql`
- [Official Download](https://www.postgresql.org/download/)

## Cloud
### AWS
Create a free-tier RDS instance in the cloud on Amazon Web Services.
1. Sign up for an account on aws.amazon.com
2. Create an RDS ([tutorial](https://aws.amazon.com/getting-started/tutorials/create-connect-postgresql-db/))

### ElephantSQL/Heroku
Alternatively, use an alternative cloud service provider like [ElephantSQL](https://www.elephantsql.com/docs/index.html) or [Heroku](https://www.heroku.com/postgres).

## Docker
Docker is a containerization tool written in Go to create lightweight containers running isolated file systems and processes. Docker can be run on non-Enterprise Windows using Docker toolbox (soon with WSL2 on Windows 10 Home), or on a Cloud EC2 linux instance.

### Installation
To install the latest version however, it is recommended to follow the official [Docker Installation](https://docs.docker.com/engine/install/centos/) documentation:

```bash
sudo yum install -y yum-utils
sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
sudo yum install docker-ce docker-ce-cli containerd.io
sudo systemctl start docker
```

Run `docker`'s hello-world container to verify installation:
>sudo docker run hello-world

### Permissions
Docker requires super user permissions and must be run with the `sudo` command by default. This can be bypassed for convenience by adding your user to the docker unix group:
>sudo usermod -aG docker <USER>

Log out, then log back in to see the changes. If successful, the following command will now work:
>docker run hello-world

### Example: PostgreSQL Server
To run a simple Postgres server instance:
>docker run -p [port]:5432 postgres

Where [port] is your choice of port. A common port is 5432, a default for many Postgres databases:
>docker run -p 5432:5432 postgres

To run a database as a background process, use the `-d` switch:
>docker run -d -p 5432:5432 postgres

It's a good idea to label a database with the `--name` switch:
>docker run -d --name my_postgres -p 5432:5432 postgres

To see running containers, use:
>docker ps

To stop a container, run:
>docker stop <CONTAINER-NAME-OR-ID>

### Running PostgreSQL from a Dockerfile
To create a custom postgres database, create a file named `Dockerfile`:
```Dockerfile
FROM postgres:10
ENV POSTGRES_USER hello-postgres
ENV POSTGRES_PASSWORD hello-postgres
ADD init.sql /docker-entrypoint-initdb.d
EXPOSE 5432
```

Where init.sql is an optional `.sql` script file in the same directory as your Dockerfile. Use `ENV` to set the username and password as needed. Both `ENV` lines can be omitted, causing the username to default to `postgres` and no password required.

To build an image from the Dockerfile:
>docker build -t demo-postgres .

Where `demo-postgres` is the name you wish to give this image. Then to run the build:
>docker run -p 5432:5432 -d demo-postgres

Remember to expose the ports and use any desired flags.

### Connecting to a Docker PostgreSQL database with `psql`
With your Docker postgres image built and a container running, use `docker exec` to run the `psql` tool on the running container:
>docker exec -it demo-postgres psql -U hello-postgres

Enter your Postgres username after `-U` (`postgres` by default if no `POSTGRES_USER` was set) and enter your password when prompted.