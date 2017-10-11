Setup local development environment.

```
mkdir MyVagrant && cd MyVagrant
mkdir MyCentOS && cd MyCentOS
vagrant init bento/centos-6.8
vi Vagrantfile # IP編集
vagrant up
vagrant ssh
sudo yum -y install git
git clone https://github.com/nuovotaka/centos6.git
cd centos6
./run.sh
exec $SHELL -l
```
