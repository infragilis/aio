# aio

ubuntu 16.4 
1  apt-get update 
2  apt-get dist-upgrade 
3  reboot
4  git clone https://opendev.org/openstack/openstack-ansible     /opt/openstack-ansible
5  cd /opt/openstack-ansible/
6  git tag -l
7  git checkout queens
8  git checkout queens-em
9  scripts/bootstrap-ansible.sh
10  export SCENARIO='aio_lxc'
11  scripts/bootstrap-aio.sh

copy and mangle the cinder.conf
/etc/openstack_deploy/conf.d/cinder.conf

mkdir /etc/cinder
/etc/cinder/nfs_shares_volume1
192.168.0.42:/var/nfs/general

# cd /opt/openstack-ansible/playbooks
# openstack-ansible setup-hosts.yml
# openstack-ansible setup-infrastructure.yml
# openstack-ansible setup-openstack.yml

/etc/ssh/sshd.config  (set Passwordauth to yes)
