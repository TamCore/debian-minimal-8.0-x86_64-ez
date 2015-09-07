# OpenVZ EZ Template Debian 8.0 Minimal x86_64
## Instructions
```
cd ~
git clone https://github.com/TamCore/debian-minimal-8.0-x86_64-ez.git
cd debian-minimal-8.0-x86_64-ez
cp -v os_* ~/rpmbuild/SOURCES
rpmbuild -v -bb debian-minimal-8.0-x86_64-ez.spec
rpm -Uvh ~/rpmbuild/RPMS/noarch/debian-minimal-8.0-x86_64-ez-*.el7.centos.noarch.rpm
vzpkg create cache debian-minimal-8.0-x86_64
```
