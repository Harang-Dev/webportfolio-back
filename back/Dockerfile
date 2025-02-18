FROM node:20 
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install
RUN npm install -g pm2
COPY . .
EXPOSE 8000
CMD ["pm2-runtime", "index.js"]