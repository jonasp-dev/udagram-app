FROM node:12

#Create app directory
WORKDIR /usr/src/app

#Install app dependencies 
#A wildcard is used to ensure both package.json AND package-lock.json are copied
COPY package*.json ./
RUN npm ci

#Bundle app source
COPY . .
Expose 8080
CMD ["npm", "run", "prod"]
