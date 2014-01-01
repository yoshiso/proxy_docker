#ProxyDocker

You will ssh to connect to the DockerContainer via Vagrant from Mac.


##Requirements

Vagrant,VirtualBox


##Installation

git clone git@github.com:yss44/proxydocker.git ~/.proxydocker

##Usage

ProxyDocker additional commands:
  ssh [docker ip] [docker port]                   SSH Docker Container in Vagrant
  setup [vm ip] [vm port] [vm username]
               [container's private key path]     Setup Docker VM
  reset                                           Reset settings
  remote list                                     Show Running Docker Container IPs
  help                                            Help for ProxyDocker


1. Setup ProxyDocker

##License

MIT License. Copyright 2014 Sho Yoshida([@yoshiso44](https://twitter.com/yoshiso44))


##Contributing

1. Fork it ( http://github.com//simple_todo/fork )
2. Create your feature branch (git checkout -b my-new-feature)
3. Commit your changes (git commit -am 'Add some feature')
4. Push to the branch (git push origin my-new-feature)
5. Create new Pull Request