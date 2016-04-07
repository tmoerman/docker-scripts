FROM sequenceiq/hadoop-docker:2.7.1
MAINTAINER VDA-LAB

RUN echo 'VDA-LAB Hadoop Image'
RUN rpm -e cracklib-dicts --nodeps
RUN yum install -y wget nano cracklib-dicts

# Export hadoop executables
RUN echo "export PATH=$PATH:/usr/local/hadoop/bin" >> etc/profile