
## Build a Docker Image

Create a `Dockerfile`:

```Dockerfile
FROM node:alpine

# Create app directory
WORKDIR /usr/src/app

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY package*.json ./

RUN npm install
# If you are building your code for production
# RUN npm ci --only=production

# Bundle app source
COPY . .

EXPOSE 8080
CMD [ "node", "server.js" ]
```

## Usage in `docker-compose`

```yaml
services:
  app:
    restart: on-failure
    build:
      context: .
      dockerfile: app.Dockerfile
    image: 'node:alpine'
    volumes:
      - './app.js:/usr/src/app.js'
    command: 'node app.js'
```

Note the mounting point should be consistent with the `Dockerfile`.

See also [[docker.compose]]
