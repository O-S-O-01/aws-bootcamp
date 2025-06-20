
FROM node:16.18

# Set environment variable
ENV PORT=3000

# Set working directory
WORKDIR /app

# Install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the code
COPY . .

# Expose port for development server
EXPOSE ${PORT}

# Start React app
CMD ["npm", "start"]
