# aio

ubuntu 16.4  
1  apt-get update  
2  apt-get dist-upgrade  
3  reboot  
4  git clone https://opendev.org/openstack/openstack-ansible     /opt/openstack-ansible  
5  cd /opt/openstack-ansible/  
6  git tag -l  
8  git checkout queens-em  
9  scripts/bootstrap-ansible.sh  
10  export SCENARIO='aio_lxc'  
11  scripts/bootstrap-aio.sh  
  
copy and mangle the cinder.yml  
/etc/openstack_deploy/conf.d/cinder.yml  
  
cd /opt/openstack-ansible/playbooks  
openstack-ansible setup-hosts.yml  
openstack-ansible setup-infrastructure.yml  
openstack-ansible setup-openstack.yml  
  
/etc/ssh/sshd.config  (set Passwordauth to yes)  on your aio host  
