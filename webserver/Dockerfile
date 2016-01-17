FROM kumarsarath588/ansible:latest

ADD ansible /srv/webserver

WORKDIR /srv/webserver

RUN ansible-playbook site.yml -c local

EXPOSE 22 3000 80

ENTRYPOINT ["/usr/local/bin/apachectl", "-DFOREGROUND"]
