FROM node:20-alpine

WORKDIR /app

# Copy package.json dan install dependencies
COPY package*.json ./
RUN npm install

# Copy seluruh source code project
COPY . .

# Build project Next.js
RUN npm run build

# Buka port 300011
EXPOSE 3000

# Jalankan aplikasi
CMD ["npm", "start"]
# Trigger dinamis
