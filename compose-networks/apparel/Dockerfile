FROM node
WORKDIR app
RUN npm install -g nodemon
RUN npm install -g dotenv
COPY package.json .
RUN npm install
RUN mv /app/node_modules /node_modules
COPY . .
EXPOSE 80
CMD ["nodemon", "server.js"]