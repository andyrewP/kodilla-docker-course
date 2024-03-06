FROM node:18-alpine

WORKDIR /app

COPY . .

EXPOSE 5001

RUN npm install express

CMD ["npm", "run", "start"]