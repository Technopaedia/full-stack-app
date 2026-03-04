# Serve static HTML with nginx
FROM nginx:alpine

# Remove default nginx content
RUN rm -rf /usr/share/nginx/html/*

# Copy static site into nginx web root
COPY index.html /usr/share/nginx/html/

# Expose HTTP port
EXPOSE 80

# nginx runs in foreground by default
CMD ["nginx", "-g", "daemon off;"]
