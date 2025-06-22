
FROM node:18

# Set environment variable
ENV PORT=3000

# Set working directory
WORKDIR /app

# Install dependencies
RUN npm config set registry https://registry.npmmirror.com
COPY package*.json ./
RUN npm install

# Copy the rest of the code
COPY . .

# Expose port for development server
EXPOSE ${PORT}

# Start React app
CMD ["npm", "start"]
