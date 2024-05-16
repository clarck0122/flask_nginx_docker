# Use the official Nginx image as a parent image
FROM nginx

# Copy nginx configuration file
COPY nginx.conf /etc/nginx/nginx.conf

# Expose port 80
EXPOSE 80

# CMD to start Nginx
CMD ["nginx", "-g", "daemon off;"]
