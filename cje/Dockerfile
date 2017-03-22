#Questions about open-source Jenkins are now based on Jenkins 2.19.4
 
FROM jenkins: 2.19.4
COPY plugins.txt /plugins.txt

#RUN /usr/local/bin/plugins.sh /plugins.txt

COPY ref /usr/share/jenkins/ref

# create a private SSH key to attach slaves
RUN mkdir "/usr/share/jenkins/ref/slaves" && ssh-keygen -N '' -t rsa -f "/usr/share/jenkins/ref/slaves/id_rsa"
