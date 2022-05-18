FROM node:4.6 as unittest
WORKDIR /app
ADD . /app
RUN echo "unit test"
RUN npm install
EXPOSE 3000
CMD npm start

FROM node:4.6 as coverageandstatanly
WORKDIR /app
ADD . /app
RUN echo "coverage and static analysis"
RUN npm install
EXPOSE 3000
CMD npm start

FROM node:4.6 as uitest
WORKDIR /app
ADD . /app
RUN echo "UI tests"
RUN npm install
EXPOSE 3000
CMD npm start

FROM node:4.6 as finalartifact
WORKDIR /app
ADD . /app
RUN echo "Final artifact"
RUN npm install
EXPOSE 3000
CMD npm start
