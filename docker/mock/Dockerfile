FROM node:10.15.0

WORKDIR /data
RUN npm install -g json-server
CMD json-server --watch db.json -m middleware.js --port 80 --host 0.0.0.0