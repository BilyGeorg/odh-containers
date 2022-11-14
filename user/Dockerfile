# 1. pick a Node 16 image
FROM node:16-alpine

# 2. set a working directory
WORKDIR /app

# 3. declare all the environemnt variables needed
ENV DATABASE_HOST=localhost
ENV DATABASE_PORT=5432
ENV DATABASE_NAEM=user
ENV DATABASE_USERNAME=g0620_team1_hacker4
ENV DATABASE_PASSWORD=lloydsHack1!
ENV CONFIG_FILE_PATH=foo

# 4. copy the app into the work directory
ADD . app
COPY ["package.json", "package-lock.json*", "./"]

# 5. install all the packages needed for NodeJS
RUN npm install 

# 6. expose the port needed
EXPOSE 3000 

# 7. start the app
ENTRYPOINT [ "nodejs", "indx.js" ]


# # syntax=docker/dockerfile:1
# FROM node:12.18.1
# ENV NODE_ENV=production

# WORKDIR /app

# COPY ["package.json", "package-lock.json*", "./"]

# RUN npm install --production

# COPY . .

# CMD [ "node", "server.js" ]