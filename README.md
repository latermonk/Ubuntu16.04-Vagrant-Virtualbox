# Ubuntu16.04-Vagrant-Virtualbox

# vagrant  
## Remove old version vagrant 
``` sudo apt-get remove --auto-remove vagrant ```
``` rm -r ~/.vagrant.d ```



## Install new version
```
wget https://releases.hashicorp.com/vagrant/1.9.1/vagrant_1.9.1_x86_64.deb
sudo dpkg -i vagrant_1.9.1_x86_64.deb 
vagrant version
```


# virtualbox

## Remove Virtualbox old version  

```  sudo apt-get remove virtualbox-\*   ```  
```  sudo apt-get purge virtualbox-\*    ```



#  successful version

ubuntu 16.04 + vagrant 2.0.3 + virtualbox 5.2      


## vagrant:
https://www.vagrantup.com/downloads.html   

```
wget https://releases.hashicorp.com/vagrant/2.0.3/vagrant_2.0.3_x86_64.deb    

```

## virtualbox:

https://www.virtualbox.org/wiki/Linux_Downloads

```
wget https://download.virtualbox.org/virtualbox/5.2.10/virtualbox-5.2_5.2.10-122088~Ubuntu~xenial_amd64.deb

```


```
sudo  apt install  vagrant_2.0.3_x86_64.deb 

sudo  apt install  virtualbox-5.2_5.2.10-122088~Ubuntu~xenial_amd64.deb

```


## Test centos/7 system

###  离线下载 centos 7 镜像

官方商店：
https://app.vagrantup.com/boxes/search


CentOS7-vgrant
https://app.vagrantup.com/centos/boxes/7   

CentOS7-official
https://cloud.centos.org/centos/7/vagrant/x86_64/images/  




###  把镜像导入系统

```
vagrant box add CentOS-xxx-xxx.box  --name centos/7

```

###  测试系统
```

mkdir  centos7_Test
cd     centos7_Test
vagrant init centos/7   -> generate Vagrantfile
vagrant up

```






