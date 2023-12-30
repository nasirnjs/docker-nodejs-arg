server.js file env has been set *app.listen(process.env.PORT);* that are pass via cli --env-file project root directory.


`docker build --build-arg NODE_VERSION=16 -t my-node-app:0.2 .`\
`docker run -p 8080:8000 -e PORT=8000 nasirnjs/nodejs:0.2`\
or\
`docker run -p 8080:8000 --env-file .env nasirnjs/nodejs:0.2`


Now Browse `http://localhost:8080`

Check container ID and exec into container.\
`docker ps`

Exec to container.\
`docker exec -it 88c /bin/bash`

Check node version.\
` node -v`