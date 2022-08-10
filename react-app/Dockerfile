# Pull official version of node image
FROM node:latest


#Set working directo
WORKDIR /app

# add `/app/node_modules/.bin` to $PATH
ENV PATH /app/node_modules/.bin:$PATH

# copy dependencies
COPY . ./

RUN npm install --silent
RUN npm install react-scripts@3.4.1 -g --silent


CMD ["npm", "start"]
