FROM node:alpine
LABEL maintainer="edmondmgodwin@outlook.com"
WORKDIR /app
RUN adduser -S uiapp
COPY . .
RUN npm install
USER uiapp
CMD [ "npm", "start" ]
