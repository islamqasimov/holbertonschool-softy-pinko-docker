FROM nginx:latest

# Copy front-end files into nginx document root
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Replace default nginx config
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
