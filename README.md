# Docker-projects
The Infrastructure projects on docker 
## Getting Started 

Get ready with the following stuff before diving into **docker-compose.yml** file.

## Install software :

- **Installing docker and docker-compose:**

  - Head to the [link](https://docs.docker.com/compose/install/). It will guide you to download and install docker-compose.

- **Installing httpd**

  - Go to the following [link](http://httpd.apache.org/docs/2.4/install.html) to download and install httpd. You can configure `httpd.conf` file.
  
## Running the docker-compose :

Create a directory and paste the given `docker-compose.yml` file into the directory. In the Terminal, head to the directory and run:

> `docker-compose up -d`

❗ Here `-d` is an option to run docker in background. You can omit it if not required. ❗

## Connecting to the database remotely from host :

- For this, you need to install `mysql` and `mariadb` software on the host o.s of docker.

  > **Note:** mysql and mariadb are conflicting packages. You need to enter `--allowerasing` option to overcome the issue.
  
- Run the following and find the IP address of mariadb container:

  > docker inspect `CONTAINER ID of mariadb`

- Run the following to connect to the mariadb database remotely :

  > mysql -h `IP of mariadb` -u `username of mariadb` -p`password of mariadb`

- If your mariadb is correctly working, you will be redirected to `mariadb shell` and you can run sql commands like `show databases;`, `show tables;`, `exit;`  etc.,

## Author :
  -> Syed Faheemuddin
  
  ->Gmail: syedfaheemuddin456987@gmail.com
  
  ->Linked-in : https://www.linkedin.com/in/syed-faheem-96b677196/

