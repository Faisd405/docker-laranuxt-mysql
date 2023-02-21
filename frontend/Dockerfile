FROM node:18-alpine

WORKDIR /app/frontend

# Copy lock files if file exists
COPY package.json yarn.lock* package-lock.json* ./

# Install dependencies
RUN yarn install

# Copy source code
COPY . .

# Build app
CMD ["yarn", "dev"]