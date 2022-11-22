FROM node:8.7-alpine
LABEL maintainer="edmondmgodwin@outlook.com"
WORKDIR /app
RUN adduser -S uiapp
COPY . .
RUN npm install
USER uiapp
#run command
CMD [ "npm", "start" ]
