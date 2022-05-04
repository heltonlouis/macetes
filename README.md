# macetes
### Este repositório tem alguns erros e suas soluções em frameworks, servidores, linux, etc..

#### ERRO SSH
##### Unable to negotiate with 192.168.0.102 port 22: no matching host key type found. Their offer: ssh-rsa,ssh-dss

###### A solução:
```sh
sudo apt update
```
```sh
cd ~
```
```sh
cd .ssh/
```
```sh
ls
```
```sh
sudo vim config
```
*pressione i para entrar no modo de edição*
*coloque os seguintes parametros*
```sh
HostkeyAlgorithms ssh-dss,ssh-rsa
```
```sh
KexAlgorithms +diffie-hellman-group14-sha1,diffie-hellman-group1-sha1
```
*para sair pressione esc, logo em seguida :wq (w - salva, q - sair)*
```sh
cd ~
```
```sh
sudo apt update
```
