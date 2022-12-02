FROM node:16.18.1-alpine3.16
RUN mkdir -p /src/app
WORKDIR /src/app
ENV CI=true
COPY package.json /src/app/
RUN npm install 
COPY . /src/app
#RUN npm run build
EXPOSE 3000
CMD [ "npm", "run", "start" ]