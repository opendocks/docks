## Docker Files and Dependencies

Repository Included

### Docker Files For

1. Apache
2. Nginx
3. PHP-FPM
4. MySQL
5. Workspace

### How to use for project
1. Create an empty directory say it <R> on you machine
2. Clone this repo in newly created directory
3. Create code <C> & data <D> sub directories
4. Copy all you application code to newly created code sub directory
5. Set html root to match path in code sub directory, in the file /dock.d/conf.d/apache/sites/apache.conf 
6. Copy /dock.d/source.env in the <R> directory and rename to .env
7. Updates any path in .env file if needed
8. Search and update proj.name to your project name, in dock.d directory
9. Copy /dock.d/docker-compose.yaml in the <R> directory
10. Adjust docker-compose.yaml service as per your requirements


### Useful Commands

Docker compose useful commands
   
To build/start all services
```bash
docker-compose up
```
  
To build/start first time
```bash
docker-compose up apache php-fpm mysql
```

To build/rebuild explicitly
```bash
docker-compose up --build apache 
```

Close all running Containers
```bash
docker-compose stop
```

To stop single container do:
```bash
docker-compose stop {container-name}
```

To stop and remove all containers:
```bash
docker-compose down
```

To stop and remove single containers:
```bash
docker-compose down {container-name}
```

To enter container terminal window
```bash
docker exec -it {container-name} bash
```
