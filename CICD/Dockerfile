FROM node:12.18.3 as builder

RUN mkdir /app
WORKDIR /app

EXPOSE 3000

COPY . /app

RUN ls -al /app
RUN echo $PWD
ENV PATH /app/node_modules/.bin:$PATH
CMD ["npm", "start"]