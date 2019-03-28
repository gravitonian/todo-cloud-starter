# Development image with all the Node.js stuff in it
FROM node:8.15.0

# Set working directory, will be created if it does not exist
WORKDIR /usr/src/app

# Install application dependencies
COPY package.json .
RUN npm install

# Copy application code
COPY . .

# Info to devs and others that this container needs to have port 4200 exposed externally,
# i.e. this instruction does not do anything more than info
EXPOSE 4200

# Start app
CMD ["npm", "start"]
