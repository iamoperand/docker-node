# docker-node

Node app deployed using Docker :)


### Using the Docker image
```
docker pull iamoperand/node
```


### Other Useful Commands

- **List Containers**: 
```
docker ps -a
```

- **Remove Containers**: 
```
docker rm <container_id>
```

-container_id: only the initials that make it differentiable from other ids. Generally, the first 2 chars.

- **List Images**:
```
docker images
```

- **Remove Images**: 
```
docker rmi <image_id>
```

-image_id: only the initials that make it differentiable from other ids. Generally, the first 2 chars.


- **Build Images**:
```
docker build -f Dockerfile -t iamoperand/node .
```

-f: specifying Docker file

-t: tag the container 


- **Run Container**:
```
docker run -d -p 8080:3000 iamoperand/node
```

-d: run it in daemon mode (run it behind the scene)

-p: specifying the port <external:internal>