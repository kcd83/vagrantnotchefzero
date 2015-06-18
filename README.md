config.vm.provision "chef_zero" is chef-solo not chef-client #5619
========

https://github.com/mitchellh/vagrant/issues/5619

`vagrant up`

```
==> default: [2015-06-18T22:18:40+00:00] INFO: Started chef-zero at chefzero://localhost:8889 with repository at /tmp/vagrant-chef/0f366ceb60019e79e27a5854b52ec1bb, /tmp/vagrant-chef/cookbooks
==> default:   One version per cookbook
==> default:   environments at /tmp/vagrant-chef/73294868f9e48523eb71d23c2fcb835d/environments
==> default:
==> default: [2015-06-18T22:18:40+00:00] INFO: Forking chef instance to converge...
==> default: [2015-06-18T22:18:40+00:00] INFO: *** Chef 12.3.0 ***
==> default: [2015-06-18T22:18:40+00:00] INFO: Chef-client pid: 6480
==> default: ================================================================================
==> default: Error expanding the run_list:
==> default: ================================================================================
==> default:
==> default: Unexpected Error:
==> default: -----------------
==> default: Chef::Exceptions::IllegalVersionConstraint: Environment cookbook version constraints not allowed in chef-solo
```
