# Base image 

FROM node:10-alpine

# Create a directory to hold the application code inside the image
WORKDIR /app
# Creates an image and cd to the folder(here its node10 apline)

COPY package.json yarn.lock ./
# copy the contents of the host machine to the image

# Install app dependencies
RUN yarn install --production
#node packages are being installed for node prod envt

COPY . .
#ENTRYPOINT ["tail", "-f", "/dev/null"]
CMD ["node", "/app/src/index.js"]
#creates a server (dev server)

#build the image is docker build -t docker-101 .