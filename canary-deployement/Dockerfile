From centos:7

# mountable directory and installing httpd server for cgi scripts
RUN \
  yum update && \
  yum -y install httpd && \
  systemctl start httpd && \
  rm /var/www/html/index.html

# Working Directory
WORKDIR /var/www/cgi-bin/

# Coping cgi-python.py to /var/www/cgi-bin/
COPY cgi-python.py /var/www/cgi-bin/

EXPOSE 80

# Push the image to docker hub using the below commands
# docker container commit --author "Navaneet" nknagaraj/python-app
# docker push nknagaraj/python-app