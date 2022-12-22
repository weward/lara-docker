# Docker Image

Files
- `docker-compose.yml`
- `./docker/Dockerfile`
- `./docker/entrypoint.sh`


### Required Actions
- Configure the `.env.example` file inside the root of the laravel application
- Give privilege to the `docker/entrypoint.sh` file: 

```
// from App root, go inside docker folder
cd docker 
sudo chmod 744 entrypoint.sh

```



### Build (and run)

- `docker-compose up -d --build`


### Run (detached)

- `docker-compose up -d`

- App url: `http://localhost:8000`


### Stop 

- `docker-compose stop`



---

## Configuration

- to change the default PORT `(http://locahost:8000)`, update `ENV PORT=` inside `./docker/Dockerfile` and update the `# PHP Service` ports inside `./docker-compose.yml`



