FROM codespaces/akurath:v0.1.0
MAINTAINER Vijayboopathy E <vibe@initcron.org>

RUN apt-get update && \
    apt-get install -y software-properties-common && \
    apt-add-repository ppa:ansible/ansible -y && \
    apt-get update && \
    apt-get install -y ansible

COPY insecure_key.pem /root/.ssh/id_rsa

EXPOSE 22 8000

CMD /usr/bin/akurath run 

