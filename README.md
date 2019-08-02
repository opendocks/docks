## Docker Image Repositories

Repository Included

### Images

1. Apache Image
2. Nginx Image
3. PHP-FPM
4. MySQL
5. Workspace

### Files/Folders

1. .env-source file

      i. Copy file to new site <br/>
     ii. Rename this to .env <br/>
    iii. Edit environment variables, as per site requirement to include or exclude libs
        
2. Copy conf folder in site conf folder,under specific service 


3. docker-compose-source.yml

     i. Copy file to new site<br/>
   iii. Use docker-compose to build image/containers e.g.


### Useful Commands

Docker compose useful commands
   
To build/start all services
```bash
docker-compose up apache php-fpm mysql
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
