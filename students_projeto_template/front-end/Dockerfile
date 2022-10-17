FROM node:16

WORKDIR /app

COPY . .

RUN npm install

RUN npm run build

RUN mkdir -p /var/www/html

# Copy the build folder to the nginx folder
RUN mv build/* /var/www/html