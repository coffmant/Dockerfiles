FROM centos:latest

RUN yum -y install python-dns python-ldap python-prettytable python-devel openldap-devel git && yum clean all

RUN git clone https://github.com/peterpakos/checkipaconsistency.git

WORKDIR checkipaconsistency

pip install -r requirements.txt

ENTRYPOINT ["/checkipaconsistency/cipa"]
