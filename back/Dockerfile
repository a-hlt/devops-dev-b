FROM node:18-alpine

WORKDIR /app

# COPY prisma ./prisma

COPY package.json ./

RUN npm install

COPY . .

RUN npx prisma generate

EXPOSE 3000

ENTRYPOINT ["./entrypoint.sh"]
