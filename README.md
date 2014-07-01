# Vagrant AWS
For a list of all the configuration options see: [https://github.com/mitchellh/vagrant-aws](https://github.com/mitchellh/vagrant-aws)

## Quick Start

After installing the plugin (instructions above), the quickest way to get
started is to actually use a dummy AWS box and specify all the details
manually within a `config.vm.provider` block. So first, add the dummy
box using any name you want:

```
$ vagrant plugin install vagrant-aws
$ vagrant box add dummy https://github.com/mitchellh/vagrant-aws/raw/master/dummy.box
$ vagrant up --provider=aws
```