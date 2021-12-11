```
Author: Nguyen Trung Hau
Email: ken.hdpro@gmail.com
Facebook: http://fb.com/irf1404
```

# INSTALL DIRECTADMIN
<b>(*) PLEASE GO THROUGH THE CONFIGURATION STEPS BEFORE INSTALLATION [HERE](https://github.com/irf1404/DACONFIG)</b>
```
# Directadmin 1.443
wget -O setup.sh "https://raw.githubusercontent.com/irf1404/DA/master/da-1443.sh" && chmod +x setup.sh && ./setup.sh 2>&1|tee directadmin_inѕtall.log

# Directadmin 1.532 For Centos6
wget -O setup.sh "https://raw.githubusercontent.com/irf1404/DA/master/da-1532-centos6.sh" && chmod +x setup.sh && ./setup.sh 2>&1|tee directadmin_inѕtall.log

# Directadmin 1.604 For Centos7
wget -O setup.sh "https://raw.githubusercontent.com/irf1404/DA/master/da-1604-centos7.sh" && chmod +x setup.sh && ./setup.sh 2>&1|tee directadmin_inѕtall.log

```

# NULL DIRECTADMIN
```
#!/bin/sh

LICENSE=/usr/local/directadmin/conf/license.key
DACONF_FILE=/usr/local/directadmin/conf/directadmin.conf

rm -rf $LICENSE
wget -O $LICENSE "https://raw.githubusercontent.com/irf1404/DACONFIG/master/license.key"

chmod 600 ${LICENSE}
chown diradmin:diradmin ${LICENSE}

if [ -s ${LICENSE} ] && [ -s ${DACONF_FILE} ]; then
	echo 'action=directadmin&value=restart' >> /usr/local/directadmin/data/task.queue.cb
	/usr/local/directadmin/dataskq --custombuild
fi

exit 0;

https://raw.githubusercontent.com/irf1404/DA/master/da-xxxx-linux64.tar.gz
```