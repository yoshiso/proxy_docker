#ProxyDocker

You will ssh to connect to the Docker Container via Vagrant from Mac.


##Requirements

Vagrant, VirtualBox, Docker v7.2


##Installation

    git clone git@github.com:yss44/proxy_docker.git ~/.proxy_docker
    echo 'export PATH="~/.proxy_docker/bin:$PATH"' >> .bashrc 
    source ~/.bashrc


##Usage

```
ProxyDocker additional commands:

  ssh [docker ip] [docker port]                   SSH Docker Container in Vagrant
  setup [vm ip] [vm port] [vm username]
               [container's private key path]     Setup Docker VM
  reset                                           Reset settings
  remote list                                     Show Running Docker Container IPs
  help                                            Help for ProxyDocker
```

###Setup ProxyDocker

```
Setting up proxydocker. proxydocker setup.
vm ip          :   VirtualBox private ip
vm port        :   VirtualBox ssh port(default 22)
vm username    :   VirtualBox user(default vagrant)
container's private key path : IdentityFile path for docker container.
```

    proxydocker setup 192.168.33.10 22 vagrant ~/.ssh/privatekey

###SSH access to container

```
docker ip   :   Docker container's ip in VirtualBox
docker port :   Docker container's port
```

    proxydocker ssh 172.17.0.10 user

##License

MIT License. Copyright 2014 Sho Yoshida([@yoshiso44](https://twitter.com/yoshiso44))


##Contributing

1. Fork it ( http://github.com//simple_todo/fork )
2. Create your feature branch (git checkout -b my-new-feature)
3. Commit your changes (git commit -am 'Add some feature')
4. Push to the branch (git push origin my-new-feature)
5. Create new Pull Request