# how-to-install-apache-on-centos
how to install apache on centos

## Install Apache
```
sudo yum clean all
sudo yum -y update
sudo yum -y install httpd
```

## Disable firewall
```
sudo firewall-cmd --permanent --add-port=80/tcp
sudo firewall-cmd --permanent --add-port=443/tcp
sudo firewall-cmd --reload
```

## Start apache
```
sudo systemctl start httpd
sudo systemctl enable httpd
sudo systemctl status httpd
sudo systemctl stop httpd
```
