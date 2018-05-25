FROM centos:latest

RUN yum -y install python-dns python-ldap python-prettytable git && yum clean all

RUN git clone https://github.com/peterpakos/checkipaconsistency.git

ENTRYPOINT ["/checkipaconsistency/cipa"]
