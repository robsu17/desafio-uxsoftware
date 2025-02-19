FROM ubuntu:22.04

WORKDIR /app

RUN apt-get update && apt-get install -y \
  openssl \
  libssl-dev \
  curl \
  gnupg2 \
  ca-certificates \
  lsb-release \
  && rm -rf /var/lib/apt/lists/*

RUN curl -fsSL https://deb.nodesource.com/setup_20.x | bash - && \
  apt-get install -y nodejs

RUN npm install -g pm2@latest 

COPY package.json package-lock.json ./

COPY prisma ./
COPY .env ./

RUN npm install 

COPY . .

RUN npm run build

EXPOSE 3000

CMD ["pm2-runtime", "ecosystem.config.js"]