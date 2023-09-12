# Use the devopsedu/webapp base image
FROM devopsedu/webapp

# Install the mysql PHP extension
RUN apt-get update && apt-get install -y php-mysql

# Copy your application files to the container's directory
COPY . /var/www/html/

# Expose port 80 for web traffic (this is already defined in the base image)

# Start the web server
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
