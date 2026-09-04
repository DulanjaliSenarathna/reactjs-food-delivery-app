#using the smallest image of nodejs 

FROM node:22-alpine

WORKDIR /app

#copying the package files

COPY package*.json ./

#installing dependenices keppt inside package-lock.json which gets stored into node_modules

RUN npm ci

#copies newly added packages

COPY . . 

#my express listens on port 4000

EXPOSE 4000

# now run the main applicaiton

CMD ["npm","run","server"]




