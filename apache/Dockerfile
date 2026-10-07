FROM httpd:2.4

# Copiamos los ficheros de configuración de los Virtual Hosts
COPY ./vhosts/ /usr/local/apache2/conf/extra/

# Copiamos el contenido web saliendo un nivel hacia la raíz
COPY ../alpha/ /usr/local/apache2/htdocs/alpha/
COPY ../beta/ /usr/local/apache2/htdocs/beta/

# Añadimos la inclusión de los vhosts al fichero de configuración principal de Apache
RUN echo "Include conf/extra/alpha.conf" >> /usr/local/apache2/conf/httpd.conf
RUN echo "Include conf/extra/beta.conf" >> /usr/local/apache2/conf/httpd.conf



