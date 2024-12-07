FROM node:16 AS build

WORKDIR /app

#  Here we copy the packege.json file to docker container 
# so npm install know what exact dependencies to install
COPY package.json . 


RUN npm install

#or just add .dockerignore file to ignore node_modules 
COPY . .

EXPOSE  5050

CMD ["npm", "start"]