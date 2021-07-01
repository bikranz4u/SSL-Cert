# SSL-Cert
# Creating SSL Cert
HOSTNAME="home.com"
openssl req -new -newkey rsa:1024 -days 365 -nodes -x509 -subj "/C=US/ST=DC/L=Washington/O=BikramHome/CN=${HOSTNAME}" -keyout ${HOSTNAME}.key  -out ${HOSTNAME}.crt
