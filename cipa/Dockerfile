FROM centos:latest

RUN yum -y install epel-release

RUN yum -y install python-pip openldap-devel git gcc && yum clean all

RUN git clone https://github.com/peterpakos/checkipaconsistency.git

WORKDIR checkipaconsistency

RUN pip install -r requirements.txt

ENTRYPOINT ["/checkipaconsistency/cipa"]
