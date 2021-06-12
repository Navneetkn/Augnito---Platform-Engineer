From nginx:1.16.1

# mountable directory
VOLUME ["/var/www"]

# Working Directory
WORKDIR /var/www

# Coping index.html to /var/www/
# index.html contains "Hello SCRIBETECH"
COPY index.html /var/www

EXPOSE 8090
# Push the image to docker hub using the below commands

# docker container commit --author "Navaneet" nknagaraj/nginx:1.16.1
# docker push nknagaraj/nginx:1.16.1