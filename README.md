Setup local development environment.

```
mkdir MyVagrant && cd MyVagrant
mkdir MyCentOS && cd MyCentOS
vagrant init bento/centos-6.8
sed -i '' -e 's/# config.vm.network "private_network", ip: "192.168.33.10"/config.vm.network "private_network", ip: "192.168.33.10"/' Vagrantfile # IP編集
vagrant up
vagrant ssh
sudo yum -y update
sudo yum -y install git
git clone https://github.com/nuovotaka/centos6.git
cd centos6
./run.sh
exec $SHELL -l
```
