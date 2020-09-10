FROM node:12.18.3 as builder

# Make dir
RUN mkdir /app
WORKDIR /app

# listen port
EXPOSE 3000

# Build
COPY *.json   /app
COPY ./src    /app
COPY ./public /app
RUN ls -l /app

RUN npm install
RUN npm cache clean --force
# RUN ls -al
# RUN ls -al node_modules/
ENV PATH /app/node_modules/.bin:$PATH
CMD ["npm", "start"]
