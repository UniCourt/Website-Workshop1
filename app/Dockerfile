# Base image 
FROM node:lts-alpine

# Create a directory to hold the application code inside the image
WORKDIR /app

COPY . .

# Install app dependencies
RUN yarn install --production

#ENTRYPOINT ["tail", "-f", "/dev/null"]
CMD ["node", "/app/src/index.js"]