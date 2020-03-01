# Force Build

docker build -f Dockerfile.dev

# Run container in port 3000

docker run -p 3000:3000 <docker-id> 

# Docker volumes 
docker run -p 3000:3000 -v /app/node_modules -v $(pwd):/app <docker-id>


# docker test
docker run -it <docker-id> npm run test

# docker exec
docker exec -it <docker-id> npm run test
