FROM node:18-alpine

WORKDIR /app

COPY package*.json ./
RUN npm install && chmod -R +x node_modules/.bin

COPY . .

EXPOSE 5173

CMD ["sh", "-c", "node node_modules/vite/bin/vite.js --host 0.0.0.0 --port 5173 --strictPort"]
