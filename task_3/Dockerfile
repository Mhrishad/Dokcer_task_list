FROM node:18

WORKDIR /app

COPY ./task_3-react-app/package*.json ./

RUN npm install

COPY ./task_3-react-app .

RUN npm run build

CMD ["npm", "start"]

EXPOSE 3000
