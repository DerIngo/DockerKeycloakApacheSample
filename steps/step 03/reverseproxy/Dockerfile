FROM httpd:2.4
RUN apt update && apt install -y \
<<<<<<< HEAD
	libapache2-mod-auth-openidc
=======
	libapache2-mod-auth-openidc \
	iputils-ping \
	less \
	vim \
	httpie \ 
	locate
>>>>>>> c791ac30676a2a05859092134cda1e48608304b5
RUN cp /usr/lib/apache2/modules/mod_auth_openidc.so /usr/local/apache2/modules/
RUN mv conf/httpd.conf conf/container_httpd.conf
CMD ["httpd-foreground"]
