#A partir d'une image ubuntu
FROM ubuntu:18.04

#Installe postfix sur notre image
RUN apt-get update
RUN apt-get --no-install-recommends -y install postfix dovecot-imapd

EXPOSE 25
EXPOSE 110
EXPOSE 995
EXPOSE 143
EXPOSE 993

CMD ["sh","-c","postfix start-fg","dovecot start-fg"]