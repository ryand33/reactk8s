# set the base image to build from 
FROM node:alpine

# set the working directory
WORKDIR /app
# add `/app/node_modules/.bin` to $PATH
ENV PATH /app/node_modules/.bin:$PATH
# copy package files
COPY package.json ./
COPY yarn.lock ./
RUN npm i
# add app
COPY ./ ./
# start app
CMD ["npm", "start"]