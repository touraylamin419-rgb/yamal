FROM nginx:alpine

# Copiamos la configuración por defecto de Nginx y los certificados TLS
COPY ./conf.d/ /etc/nginx/conf.d/
COPY ./certs/ /etc/nginx/certs/
