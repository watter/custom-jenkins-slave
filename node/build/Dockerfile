FROM registry.redhat.io/openshift3/jenkins-slave-base-rhel7:latest
RUN cd /tmp

RUN curl -O https://nodejs.org/dist/v15.4.0/node-v15.4.0-linux-x64.tar.xz

RUN tar -xvf node-v15.4.0-linux-x64.tar.xz

RUN cp node-v15.4.0-linux-x64/bin/node /usr/local/bin

RUN chown -R 1001:0 $HOME && \
    chmod -R g+rw $HOME

USER 1001
