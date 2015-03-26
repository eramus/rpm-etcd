rpm-etcd
========

An RPM spec file to build and install etcd.

To Install:

`sudo yum -y install rpmdevtools && rpmdev-setuptree`

`wget https://raw.github.com/nmilford/rpm-etcd/master/etcd.spec -O ~/rpmbuild/SPECS/etcd.spec`

`wget https://github.com/coreos/etcd/releases/download/v2.0.5/etcd-v2.0.5-linux-amd64.tar.gz -O ~/rpmbuild/SOURCES/etcd-v2.0.5-linux-amd64.tar.gz`

`wget https://raw.github.com/nmilford/rpm-etcd/master/etcd.service -O ~/rpmbuild/SOURCES/etcd.service`

`wget https://raw.github.com/nmilford/rpm-etcd/master/etcd.sysconfig -O ~/rpmbuild/SOURCES/etcd.sysconfig`

`rpmbuild -bb ~/rpmbuild/SPECS/etcd.spec`
