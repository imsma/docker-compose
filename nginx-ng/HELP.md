# Deploying an Angular Project with Docker Compose and Nginx

## Building the Angular Project

Execute the following command to build your Angular project:

```
npm run build
```

## Modifying the Volume in Docker Compose

Adjust the volume in the Docker Compose configuration to point to the Angular build directory `dist`. Your configuration should look like this:

```
- ./dist/projectname:/usr/share/nginx/html
```

## Launching Docker Compose Services

To initiate the Docker Compose services, use the command below:

```
docker compose up -d
```

## Halting Docker Compose Services

To cease the operation of the Docker Compose services, employ the following command:

```
docker compose down
```
