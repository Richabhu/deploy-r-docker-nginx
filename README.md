# deploy-r-docker-nginx

Prerequisites:

    Docker
    Docker-compose

If you don't have docker, please follow the following link to download it:

```https://www.digitalocean.com/community/tutorials/how-to-install-docker-compose-on-ubuntu-18-04```

Now, once the setup is ready, run the following command to run the server

```docker-compose up -d --build```


You can check the running containers by
docker-compose ps

Once, both the containers are up, check the output by

curl http://127.0.0.1/echo

Or You can directly hit it in your browser by ur IP
http://<your-system-ip>/echo

Note, this is the REST API in R which prints the hello world.
You, can put your model API in the R_demo/api.R file and up the container by

docker-compose up -d --build

