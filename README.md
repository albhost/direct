Author: Nguyễn Trung Hậu<br>
Email: ken.hdpro@gmail.com<br>
Facebook: http://fb.com/irf1404<br>

# COMMON PRE-INSTALL COMMANDS
```
# CentOS 6
yum -y install wget tar gcc gcc-c++ flex bison make bind bind-libs bind-utils openssl openssl-devel perl quota libaio \
libcom_err-devel libcurl-devel gd zlib-devel zip unzip libcap-devel cronie bzip2 cyrus-sasl-devel perl-ExtUtils-Embed \
autoconf automake libtool which patch mailx bzip2-devel lsof glibc-headers kernel-devel expat-devel db4-devel ipset

# CentOS 7
yum -y install wget tar gcc gcc-c++ flex bison make bind bind-libs bind-utils openssl openssl-devel perl quota libaio \
libcom_err-devel libcurl-devel gd zlib-devel zip unzip libcap-devel cronie bzip2 cyrus-sasl-devel perl-ExtUtils-Embed \
autoconf automake libtool which patch mailx bzip2-devel lsof glibc-headers kernel-devel expat-devel \
psmisc net-tools systemd-devel libdb-devel perl-DBI perl-Perl4-CoreLibs perl-libwww-perl xfsprogs rsyslog logrotate \
crontabs file kernel-headers ipset
```

# INSTALL DIRECTADMIN
```
# Directadmin 1.443
wget -O setup.sh "https://raw.githubusercontent.com/irf1404/DA/master/da-1443.sh" && chmod +x setup.sh && ./setup.sh

# Directadmin 1.532 For Centos6
wget -O setup.sh "https://raw.githubusercontent.com/irf1404/DA/master/da-1532-centos6.sh" && chmod +x setup.sh && ./setup.sh

# Directadmin 1.604 For Centos7
wget -O setup.sh "https://raw.githubusercontent.com/irf1404/DA/master/da-1604-centos7.sh" && chmod +x setup.sh && ./setup.sh

```
