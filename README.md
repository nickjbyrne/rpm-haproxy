rpm-haproxy
===========

An RPM spec file to build and install the is HAProxy TCP/HTTP reverse proxy with SSL enabled.

To Build:

    sudo yum -y groupinstall "Development Tools"
    sudo yum -y install pcre-devel openssl-devel
    wget http://www.haproxy.org/download/1.5/src/haproxy-1.5.12.tar.gz -O ~/rpmbuild/SOURCES/haproxy-1.5.12.tar.gz
    rpmbuild -bb  ~/rpmbuild/SPECS/haproxy.spec --define "release 1"
