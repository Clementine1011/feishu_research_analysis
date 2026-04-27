FROM node:lts-alpine

WORKDIR /app

COPY package*.json ./
RUN npm install --only=production

COPY . .

ENV NODE_ENV=production

ARG PORT=3000
ENV PORT=${PORT}
EXPOSE ${PORT}

CMD ["npm", "start"]
