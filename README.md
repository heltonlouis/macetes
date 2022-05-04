# macetes
### Este repositório tem alguns erros e suas soluções em frameworks, servidores, linux, etc..

## ERRO SSH
### Unable to negotiate with 192.168.0.102 port 22: no matching host key type found. Their offer: ssh-rsa,ssh-dss

A solução:
  $ sudo apt update
  $ cd ~
  $ cd .ssh/
  $ ls
  $ sudo vim config
      // pressione i para entrar no modo de edição
      // coloque os seguintes parametros
      HostkeyAlgorithms ssh-dss,ssh-rsa
      KexAlgorithms +diffie-hellman-group14-sha1,diffie-hellman-group1-sha1
    
      // para sair pressione esc, logo em seguida :wq (w - salva, q - sair)

  $ cd ~
  $ sudo apt update
